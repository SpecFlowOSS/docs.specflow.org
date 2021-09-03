# Managing Licenses

We have introduced a new license model for SpecFlow+ and SpecMap. Our new licensing model is account-based instead of requiring a license key.

You need to sign up for a free personal SpecFlow account in order to use SpecFlow+ and SpecMap. [Learn more](../specflowaccount.md)

## Unregistering a License

Use the unregister option to remove a SpecFlow+ license from a user’s machine:

`specflow-plus-license unregister`

`SpecRun.exe unregister`

This is only necessary if the user will continue to have access to the machine, but should no longer be licensed to use SpecFlow+, for example if the user is no longer assigned to a project using SpecFlow+.

This step is not necessary if the user has left your organization and can no longer use the license on the machine, as the license key is written to the user’s registry. This means that re-imaging the hard drive will also remove the license.

## Register a Legacy License Key

You need to specify your license key and the licensee *(“Issued to”)* values in the command line. You should have received an email including your license key and licensee.

### Registering your license with SpecFlow+ Runner 3 or higher

If you are using SpecFlow+ Runner with .NET Core, you need to [install the SpecFlow licensing tool](https://docs.specflow.org/projects/specflow-runner/en/latest/Installation/SpecFlowPlus-Licensing-Tool.html) and use that to [register your license](https://docs.specflow.org/projects/specflow-runner/en/latest/Installation/SpecFlow.Plus.License-Commands.html).

To install the tool:

**1-** Open a command prompt.

**2-** Run the following command:

``` batch

dotnet tool install --global SpecFlow.Plus.License

```

**> Note:** If you want to install a specific version, use the --version option to specify the desired version:

``` batch

dotnet tool install --global SpecFlow.Plus.License --version

```

**3-** You can test that the installation was successful and display your license status using the following command:
specflow-plus-license about

To register your license:

Open a command prompt and use the following to register your license:

``` batch
specflow-plus-license register --licenseKey KEY --issuedTo "LICENSEE"
```

Replace the placeholders (KEY and LICENSEE) with your license key and licensee. For example:

``` batch
specflow-plus-license register --licenseKey KBh8227Ahb9382QAAA=== --issuedTo "ACME Corp."
```

**> Note:** The licensee and license key are case-sensitive.

### Registering Older Versions of SpecFlow+

Use *SpecRun.exe* or *SpecFlow.Plus.Excel.Converter.exe* (located in the /packages folder of your Visual Studio solution) to register your license. Detailed instructions can be found [here](https://specflow.org/plus/documentation/Registering-SpecFlowPlus/).

The following example uses SpecRun.exe. You can use the same syntax with SpecFlow.Plus.Excel.Converter.exe. Note that you only need to register the license once per machine, and registering the license for SpecFlow+ Runner also registers the license for SpecFlow+ Excel, and vice versa.

The syntax is as follows:

``` batch
SpecRun.exe register --licenseKey KEY --issuedTo "LICENSEE"
```

Replace the placeholders (KEY and LICENSEE) with your license key and licensee. For example:

``` batch
SpecRun.exe register --licenseKey KBh8227Ahb9382QAAA=== --issuedTo "ACME Corp."
```

**> Note:** The licensee and license key are case-sensitive!

### Displaying Your License Details

Start specflow-plus-license or SpecRun.exe from the [command line](http://www.specflow.org/plus/documentation/SpecFlowPlus-Runner-Command-Line/?_gl=1*z3l2t*_ga*MTY5OTI0NzMxNy4xNjIyMDEzOTkw*_ga_BZ55XKTXC6*MTYyMzIzNzI5MC40My4xLjE2MjMyNDU3MjkuMA..&_ga=2.43932133.1114192995.1623048727-1699247317.1622013990) with the `about` parameter to display license information, including the licensee and the date on which your upgrade period ends or your license expires.
