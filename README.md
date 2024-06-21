<h1>Version Control Dump</h1>

For version control on Github content file will be split into "Dynamic" and "Static"
Dynamic files include blueprints, bindings, scripts. Any assest that might change frequently
Static files include meshes, textures, audio, animations. Typically larger game files that dont change

<h2>Reason for File structure:</h2>
Due to the small nature of the project, we will use the github LFS for storing large assets which dont change. This will make each version control action to be more efficient as we wont be updating large files unless its neccesary.

<h2>Unreal Workflow for maintaining version control:</h2>
Due to the nature of binary files, you cant merge or compare them.
This is only a real concern is with blueprint files as most binary files are not edited once they are added like maps and assets.
If two different people work on the same blueprint file, it will create a merge conflict that wont be comparable with no way of knowing which version to take
  <h3>The Solution: Naming conventions!</h3>
  The naming convention will be very simple, every new binary asset from the list below needs to have its name start with E or A depending on who has control of that asset
  Ex: If Everest make a new blueprint it will be named "E (blueprint_name)"
  
  <h4>I will update this list with all the assets that require special naming convention</h4>
  <ul>
    <li>Blueprints</li>
  </ul>
  
  
