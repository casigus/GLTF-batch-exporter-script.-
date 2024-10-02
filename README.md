# GLTF-batch-exporter-script.-
GLTF Batch Exporter for Unreal Engine


GLTF Batch Exporter for Unreal Engine
This Python script allows you to batch export individual static mesh actors from your Unreal Engine map into .gltf format. Unlike Unreal's built-in export tools, which export all assets together as one file, this script exports each static mesh actor as a separate .gltf file. It's perfect for users who need to maintain the individuality of assets during the export process.

Features:
Exports all static mesh actors in the current level as individual .gltf files.
Customizable export folder path.
Automation for large-scale exports without manually exporting each asset.
Why Use This Script?:
Unreal Engine's built-in export tool exports everything as a single object, or you have to export one model at a time. This script solves that by allowing you to export every static mesh actor as separate files automatically.
It’s particularly useful for large projects with many static mesh assets, as it speeds up the export process and simplifies asset organization.
How to Use:
Set your custom export folder path in the script.
Run the script through Unreal’s Python console.
Each static mesh actor will be exported individually to your chosen directory in .gltf format.
This tool is ideal for developers working on large projects who need efficient, clean asset exporting. Whether you're preparing assets for external use or organizing your project, this script will save you time and frustration.

Feel free to modify this as needed, and you can attach it along with the script and instructions for a clear, professional presentation!


Instructions for Using the Script:
Set Up Your Export Path:

In the script, locate this line:
python
Copy code
export_folder = "Your/Custom/Export/Path/Here"
Replace "Your/Custom/Export/Path/Here" with the path where you want to save the exported .gltf files. For example:
python
Copy code
export_folder = "E:/batchexports/"
Running the Script:

Open the Unreal Editor.
Open the Python console by going to Window > Developer Tools > Output Log.
Paste the entire script into the input field at the bottom of the Output Log window.
Press Enter to run the script. It will export each static mesh actor from the current level as an individual .gltf file into the specified folder.
Important Notes:

Ensure that your export folder path ends with a / or \, depending on your operating system.
The script will only export static mesh actors. Other types of assets or actors will not be exported.
Make sure to run the script in the correct map or scene to avoid exporting duplicate assets from other maps.
Customizing:

If you want to modify the export options (e.g., texture coordinates, normals, etc.), you can customize the unreal.GLTFExportOptions() as needed.
You can expand the script to handle other asset types by adjusting the if isinstance(actor, unreal.StaticMeshActor) line to include additional checks.
Publishing:
You can include these instructions along with the script on platforms like GitHub or Unreal Engine forums to make it user-friendly for others!

Let me know if you'd like to tweak anything else before publishing!





