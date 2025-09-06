## Step-by-Step Explanation

1. Clone the repository: git clone https://github.com/SharkzTech/spotify-c-v2.git
   What it does: This command copies the entire project's source code from GitHub onto your computer.

   How to do it:
   - Open your terminal (PowerShell, as in your previous example).
   - Navigate to the directory where you want to store the project (e.g., cd Desktop).
   - Run the command: git clone https://github.com/SharkzTech/spotify-c-v2.git
   - This will create a new folder called spotify-c-v2 containing all the project files.

2. Install dependencies: cd spotify-c-v2 npm install
   What it does: Modern JavaScript projects rely on external libraries (called "dependencies"). The npm install command reads the package.json file you saw in the previous error and downloads all these required      libraries into a node_modules folder.

   How to do it:

   - After cloning, you must enter the project directory: cd spotify-c-v2
   - Then run the command to install the dependencies: npm install
   - You will see a lot of activity in the terminal as packages are downloaded. Wait for it to finish.

3. Create a Spotify application
   Why this is necessary: The app needs permission from Spotify to access user data (like your playlists or listening history). Spotify requires you to register your app so they know who is making the requests.      This is a crucial security step.

   How to do it:

   - Go to the Spotify Developer Dashboard and log in with your Spotify account.
   - Click "Create App".
   - Fill in the details (Name, Description). You can name it something like "My Dev Test".
   - The most important part: On the app's settings page, find the "Redirect URIs" field. Add https://localhost:5173 and click "Save". This tells Spotify that it's okay to redirect users back to your local             development server after they log in.

4. Create .env, and fill in your Spotify application's Client ID and Client Secret.
   What it is: A .env file is used to store sensitive configuration variables (like passwords/API keys) separately from your code. You should never commit this file to GitHub.

   - How to do it:
   - Inside your spotify-c-v2 project folder, create a new text file.
   - Name it exactly .env (the dot at the start is important!).
   - Open it in a text editor (like Notepad or VSCode).
   - You will need to add your credentials from the Spotify Dashboard you just created. The file should look like this:

   env
   VITE_SPOTIFY_CLIENT_ID=your_client_id_here
   VITE_SPOTIFY_CLIENT_SECRET=your_client_secret_here

   - Copy your "Client ID" and "Client Secret" from your Spotify app's page and paste them as the values, without quotes.

