<h1>Using UE5 with GitHub</h1>
For ease of use it is highly reccomended to use github desktop
<h3>Rules for interaction</h3>
I am considering creating two folders in content, "Adam" and "Everest" where all new assets/blueprints will be stored.
This will avoid a majority of merge conflict issues, The only foreseeable problem is with map files but this will be circumvented with a DEV branch that our respective branches are PR'ed to for testing before going to main
For now we will have main, dev, Adam, Everest branches. I might switch to a feature branch architechture but only after i understand unreal workflow more
Changing branch or pulling from repo while the unreal project is loaded will result in temporary freezing and a desync from git.
During which changes might not be saved correctly to your branch

<h2>Getting Cloned</h2>
In GitHub Desktop, Go to file and hit "Clone a repository"
Log in if prompted, Find "AdamCanard/LiminalGame"
Set Local path to
"C:\Users\'User'\Documents\Unreal Projects\LiminalGame"

<h2>Getting it Open</h2>
Start UE5, Liminal Game should ne in your project repo. If not message me  

<h3>Unreal Workflow for maintaining version control:</h3>
Due to the nature of binary files, you cant merge or compare them.
If two different people work on the same blueprint file, it will create a merge conflict that wont be comparable with no way of knowing which version to take
  <h3>The Solution: Seperate Folders!</h3>
  There will be an Adam Folder and an Everest Folder that each of us will create our new assest/blueprints in
  This is only for merge conflict as it will let me take incoming or current based on who made changes in what folder
  This wont solve map/levels files from merge conflicts so I am wanting to implement the dev branch for combining levels
  In the future i might seperate map/level files further if we start losing versions due to inproper merging on my part 
  
  
