# AppsEngineDoc
Starters guide to apps Engine
Setting up the development environment with Rocket Chat
1. Clone the repo.
2. cd in the rocketchat Apps engine folder and run 
    > npm install
3. Make the required changes and then to see those changes compile the project using 
    > npm run compile
4. After compiling the compiled package is stored in the definition directory and we have to use this as the local package for rocket.chat. 
 5. cd into the rocket chat directory and run 
    > meteor npm install PATH_TO_APP_ENGINE_REPO/definition
 6. Start the rocketchat server using 
    > meteor run
    
If we have made a change to the apps engine and for example made a feature in the engine and want to test that feature by making an app follow the following steps : -
1. Compile the changes in the apps-engine repository  
        > npm run compile 
2. In the directory where app is made instead of where the production package of apps-engine replace it with the local compiled version of the apps-engine
3. Then the use 
        > npm install to install local version as a package
