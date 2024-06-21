<h1>Using UE5 with GitHub</h1>
For ease of use it is highly reccomended to use github desktop
<h3>Rules for interaction</h3>
Currently seems like files are user specific. Subject to change as i understand the unreal structure
Always pull from git repo before loading the project in unreal
Changing branch or pulling from repo while the unreal project is loaded will result in temporary freezing and a desync from git.
During which changes might not be saved correctly to your branch
Put all new files into Dynamic folder, Static files will be moved to static folder during PR's

<h2>Getting Cloned</h2>
In GitHub Desktop, Go to file and hit "Clone a repository"
Log in if prompted, Find "AdamCanard/LiminalGame"
Set Local path to
"C:\Users\'User'\Documents\Unreal Projects\LiminalGame"

<h2>Getting it Open</h2>
Start UE5, Liminal Game should ne in your project repo. If not message me  

<h2>Version Control Dump</h2>

For version control on Github content file will be split into "Dynamic" and "Static"
Dynamic files include blueprints, bindings, scripts. Any assest that might change frequently
Static files include meshes, textures, audio, animations. Typically larger game files that dont change

<h3>Reason for File structure:</h3>
Due to the small nature of the project, we will use the github LFS for storing large assets which dont change. This will make each version control action to be more efficient as we wont be updating large files unless its neccesary.

<h3>Unreal Workflow for maintaining version control:</h3>
Due to the nature of binary files, you cant merge or compare them.
This is only a real concern is with blueprint files as most binary files are not edited once they are added like maps and assets.
If two different people work on the same blueprint file, it will create a merge conflict that wont be comparable with no way of knowing which version to take
  <h3>The Solution: Naming conventions!</h3>
  The naming convention will be very simple, every new asset needs to have its name start with E or A depending on who has control of that asset
  Ex: If Everest make a new blueprint it will be named "E (blueprint_name)"

  
  
