# Musify

A modern, responsive Spotify clone built with React and Vite. Musicfy delivers a seamless music browsing experience, mirroring the core functionalities of the popular streaming service. This project served as a comprehensive trail to explore and demonstrate proficiency in modern React development, state management, and API integration.

## Prerequisites 

- Node.js (v16 or higher)
- npm or yarn package manager
- A Spotify Premium Account (required for audio playback via the API)

## Installation

1. Clone the repository: git clone https://github.com/SharkzTech/spotify-c-v2.git

   - Open your terminal (PowerShell, as in your previous example).
   - Navigate to the directory where you want to store the project (e.g., cd Desktop).
   - Run the command: git clone https://github.com/SharkzTech/spotify-c-v2.git
   - This will create a new folder called spotify-c-v2 containing all the project files.

2. Install dependencies: cd spotify-c-v2 npm install
   
   - After cloning, you must enter the project directory: cd spotify-c-v2
   - Then run the command to install the dependencies: npm install
   - You will see a lot of activity in the terminal as packages are downloaded. Wait for it to finish.

3. Create a Spotify application

   - Go to the Spotify Developer Dashboard and log in with your Spotify account.
   - Click "Create App".
   - Fill in the details (Name, Description). You can name it something like "My Dev Test".
   - The most important part: On the app's settings page, find the "Redirect URIs" field. Add https://localhost:5173 and click "Save". This tells Spotify that it's okay to redirect users back to your local             development server after they log in.

4. Create .env, and fill in your Spotify application's Client ID and Client Secret.

   - Inside your spotify-c-v2 project folder, create a new text file.
   - Name it exactly .env (the dot at the start is important!).
   - Open it in a text editor (like Notepad or VSCode).
   - You will need to add your credentials from the Spotify Dashboard you just created. The file should look like this:
     
   ```
   env
    
   VITE_SPOTIFY_CLIENT_ID=your_client_id_here 
   VITE_SPOTIFY_CLIENT_SECRET=your_client_secret_here
   ```
    
   - Copy your "Client ID" and "Client Secret" from your Spotify app's page and paste them as the values, without quotes.

## License

This project is licensed under the MIT License - see the LICENSE.md file for details. Note that this project uses the Spotify API and is intended for educational purposes only. All branding and audio content are property of their respective owners.
