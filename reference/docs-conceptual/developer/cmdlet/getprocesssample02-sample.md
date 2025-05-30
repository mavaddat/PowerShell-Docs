---
description: GetProcessSample02 Sample
ms.date: 09/13/2016
title: GetProcessSample02 Sample
---
# GetProcessSample02 Sample

This sample shows how to write a cmdlet that retrieves the processes on the local computer. It
provides a `Name` parameter that can be used to specify the processes to be retrieved. This cmdlet
is a simplified version of the `Get-Process` cmdlet provided by Windows PowerShell 2.0.

## How to build the sample using Visual Studio

1. With the Windows PowerShell 2.0 SDK installed, navigate to the GetProcessSample02 folder. The
   default location is
   `C:\Program Files (x86)\Microsoft SDKs\Windows\v7.0\Samples\sysmgmt\WindowsPowerShell\csharp\GetProcessSample02`.

1. Double-click the icon for the solution (.sln) file. This opens the sample project in Visual
   Studio.

1. In the **Build** menu, select **Build Solution** to build the library for the sample in the
   default `\bin` or `\bin\debug` folders.

## How to run the sample

1. Create the following module folder:

    `[user]\Documents\WindowsPowerShell\Modules\GetProcessSample02`

1. Copy the sample assembly to the module folder.

1. Start Windows PowerShell.

1. Run the following command to load the assembly into Windows PowerShell:

    `Import-Module getprossessample02`

1. Run the following command to run the cmdlet:

    `Get-Proc`

## Requirements

This sample requires Windows PowerShell 2.0.

## Demonstrates

This sample demonstrates the following.

- Declaring a cmdlet class using the Cmdlet attribute.

- Declaring a cmdlet parameter using the Parameter attribute.

- Specifying the position of the parameter.

- Declaring a validation attribute for the parameter input.

## Example

This sample shows an implementation of the Get-Proc cmdlet that includes a `Name` parameter.

```csharp
namespace Microsoft.Samples.PowerShell.Commands
{
  using System;
  using System.Diagnostics;
  using System.Management.Automation;     // Windows PowerShell namespace

  #region GetProcCommand

  /// <summary>
  /// This class implements the Get-Proc cmdlet.
  /// </summary>
  [Cmdlet(VerbsCommon.Get, "Proc")]
  public class GetProcCommand : Cmdlet
  {
    #region Parameters

    /// <summary>
    /// The names of the processes retrieved by the cmdlet.
    /// </summary>
    private string[] processNames;

    /// <summary>
    /// Gets or sets the list of process names on which
    /// the Get-Proc cmdlet will work.
    /// </summary>
    [Parameter(Position = 0)]
    [ValidateNotNullOrEmpty]
    public string[] Name
    {
      get { return this.processNames; }
      set { this.processNames = value; }
    }

    #endregion Parameters

    #region Cmdlet Overrides

    /// <summary>
    /// The ProcessRecord method calls the Process.GetProcesses
    /// method to retrieve the processes specified by the Name
    /// parameter. Then, the WriteObject method writes the
    /// associated process objects to the pipeline.
    /// </summary>
    protected override void ProcessRecord()
    {
      // If no process names are passed to the cmdlet, get all
      // processes.
      if (this.processNames == null)
      {
        WriteObject(Process.GetProcesses(), true);
      }
      else
      {
        // If process names are passed to cmdlet, get and write
        // the associated processes.
        foreach (string name in this.processNames)
        {
          WriteObject(Process.GetProcessesByName(name), true);
        }
      } // End if (processNames...).
    } // End ProcessRecord.
    #endregion Cmdlet Overrides
  } // End GetProcCommand class.
  #endregion GetProcCommand
}
```

## See Also

- [Writing a Windows PowerShell Cmdlet](./writing-a-windows-powershell-cmdlet.md)
