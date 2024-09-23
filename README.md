# Layout Container Component for Sitecore XM Cloud

Steps to add the Layout Container Component to your XMCloud project
1.	Clone the repository

    Begin by cloning the following repository:
    https://github.com/sitecorelabs/sitecore-xmcloud-components-layout-container

2.	Copy serialized Items files
    
    Copy `layoutcontainer.module.json` file from `src`  to your repository’s `src` folder

    > *Ensure `layoutcontainer.module.json` path matches modules wildcard in `sitecore.json` in the root of project repository*

    Copy `LayoutContainer` folder from `src\items` folder to `Items` folder in your repository

    > *For XM Cloud Starter Kit, items are typically located in `src/items`*

3.	Copy Component and styles

    3.1 Copy component

    Copy `LayoutContainer.tsx` file from `src\components` folder to your `components` folder
    > *For XM Cloud Starter Kit, components are typically located in: `src\sxastarter\src\components`*

    3.2	Copy styles

    Copy `src\components\assets\sass\layout-container` folder to your repository *styles* folder  
    > *For XM Cloud Starter Kit, styles are typically located in: `src\sxastarter\src\assets\sass\components\`*

    3.3 Import styles

    For example, in XM Cloud Starter Kit 

    •	Locate the `src\sxastarter\src\assets\sass\components\index.scss` file 

    •	Import styles by adding this statement:  
    ```css
    @import "layout-container"; 
    ```

4.	Apply Items Serialization

    For example, in XM Cloud Starter Kit 
    
    •	Open the `up.ps1` file present at the repository root 

    •	Find the existing serialization command (`dotnet sitecore ser push -i RenderingHost`)

    •	Add new commands after it 
    ```powershell
    Write-Host "Pushing LayoutContainer component serialization" -ForegroundColor Green
    dotnet sitecore ser push -i LayoutContainer
    ```
    •	Run `up.ps1`

5.	Enable **`Layout container`** component for site

    •	Open `Content Editor` in your XM Cloud instance e.g. https://xmcloudcm.localhost/sitecore and navigate to your site in the content tree

    •	Under the `Presentation` section, expand `Available Renderings`

    •	Click on `Page Structure` and click `Edit` in the `Data` section

    •	In the `Page Structure` rendering, locate the `Layout Container` component

    •	Add the `Layout Container` to the `Page Structure` rendering.
     > *Path: Layout\Renderings\Feature\Headless Experience Accelerator\Layout Container*
    
    ![Layout Container Example](/guide/add-layout-rendering-example.png)

6. Verify in XM Cloud Pages

    •	Navigate to your site in XM Cloud Pages

    •	The `Layout Container` component should now appear in the `Page Structure` section