# Movie Recommendation Engine

This project is a movie recommendation engine built using Streamlit. It allows users to select a movie and receive recommendations based on their choice. The application fetches movie posters and displays them alongside the recommended movie titles.

## Project Structure

- `app.py`: Contains the main application code for the movie recommendation engine, including functions to fetch movie posters and recommend movies.
- `requirements.txt`: Lists the dependencies required for the project, including libraries such as Streamlit and requests.
- `README.md`: Documentation for the project, including setup and running instructions.

## Setup Instructions

To set up and run the application locally, follow these steps:

1. **Clone the Repository**:
   ```
   git clone <repository-url>
   cd Movie_recommendation_engine
   ```

2. **Install Dependencies**:
   Make sure you have Python installed, then install the required packages:
   ```
   pip install -r requirements.txt
   ```

3. **Run the Application**:
   Start the Streamlit application:
   ```
   streamlit run app.py
   ```

4. **Open in Browser**:
   After running the command, a new tab will open in your default web browser displaying the movie recommendation engine.

## Deployment on Vercel

To deploy this project on Vercel, follow these steps:

1. **Create a Vercel Account**: Sign up for a Vercel account if you don't have one.

2. **Install Vercel CLI**: Install the Vercel CLI globally using npm:
   ```
   npm install -g vercel
   ```

3. **Prepare Your Project**:
   - Ensure your `requirements.txt` file is complete with all necessary dependencies.
   - Modify `app.py` to include a `main` function that runs the Streamlit app if it's not already present.

4. **Create a Vercel Configuration File**: Create a `vercel.json` file in the root of your project with the following content:
   {
     "builds": [
       {
         "src": "app.py",
         "use": "@vercel/python"
       }
     ],
     "routes": [
       {
         "src": "/(.*)",
         "dest": "app.py"
       }
     ]
   }

5. **Deploy Your Project**:
   - Open your terminal and navigate to your project directory.
   - Run the following command to deploy:
     ```
     vercel
     ```
   - Follow the prompts to link your project to your Vercel account and deploy it.

6. **Access Your Deployed App**: After deployment, Vercel will provide a URL where your app is hosted. You can access your movie recommendation engine from that URL.

Make sure to test your application after deployment to ensure everything is working as expected.