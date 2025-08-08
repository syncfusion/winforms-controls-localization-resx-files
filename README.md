# Localization of Syncfusion® WF controls using .resx files      

This respository contains the default resources file (.resx) of Syncfusion Windows Forms libraries. You can use this resource files to localize the strings for any selected language.

## Localization of Syncfusion Windows Forms Controls

Localization is the process of translating the application resources into different language for the specific cultures. You can localize the syncfusion Windows Forms Controls by adding resource file for each language.

### Changing application culture

When you are changing the application culture, then you can localize the application based on application culture by creating .resx file.
  
```
public Form1()
{
    System.Threading.Thread.CurrentThread.CurrentCulture = new System.Globalization.CultureInfo("de-DE");
    System.Threading.Thread.CurrentThread.CurrentUICulture = new System.Globalization.CultureInfo("de-DE"); 
    InitializeComponent();
}
```

## Creating .resx files

You can create .resx files for any languages by following steps,

1) Right click your project and click `New Folder` and set name as `Resources`.

2) Add default resource file of libraries you are using to `Resources` folder.

> Consider you are using `SfDataGrid` control in your application. Then you need to copy and include `Syncfusion.SfDataGrid.WinForms.resx` (since `SfDataGrid` present in `Syncfusion.SfDataGrid.WinForms` library) file in your application under `Resources` folder. So, now you can know the key names and values of default strings used in `Syncfusion.SfDataGrid.WinForms.dll` library.

![WF DataGrid Localization](https://help.syncfusion.com/windowsforms/Localization_images/winforms-default-resx-file.png)

3) Now, right click on `Resources` folder and select `Add` and then `New Item`. In the `Add New Item` wizard, select `Resources File` option and name the file name as `Syncfusion.SfDataGrid.WinForms.<culture name>.resx`. For example, you have to give name as `Syncfusion.SfDataGrid.WinForms.de-DE.resx` for `German` culture. In the same way, add new resource files for other libraries used in your application.

![WF DataGrid Localization](https://help.syncfusion.com/windowsforms/Localization_images/winforms-adding-resource-file.png)

4) Now, select `Add` and add resource file for german culture in `Resources` folder.

![WF Localization using .resx file](https://help.syncfusion.com/windowsforms/Localization_images/winforms-resx-file-to-localize.png)

5) Now, you can copy the key names from default resource files and change its corresponding value based on the culture, the resource file targets.

![WF Localization using key value of .resx file](https://help.syncfusion.com/windowsforms/Localization_images/winforms-localized-resx-file.png)

> Download demo from [GitHub](https://github.com/SyncfusionExamples/winforms-datagrid-localization)

## Editing default culture settings 

You can change the default string of any control by adding the default .resx files ([from GitHub](https://github.com/syncfusion/winforms-controls-localization-resx-files)) to `Resources` folder of your application. Syncfusion Windows Forms controls reads the default string from the .resx files of application if its added. 