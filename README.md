# AI Blog Generator

This project is an AI-powered blog generator built with Python and Django. It allows users to generate high-quality blog articles from YouTube videos using artificial intelligence. This project was created by following a [YouTube tutorial](https://www.youtube.com/watch?v=_IC6wEt6KRc&t=9134s) to learn Python and Django.

## Features

- User authentication (login, signup, logout)
- Generate blog articles from YouTube video links
- View all generated blog articles
- View details of individual blog articles

## APIs Used

This project utilizes the following APIs:

1. **OpenAI API**: Used to generate blog content from YouTube video transcriptions.

   - [OpenAI API Documentation](https://beta.openai.com/docs/)

2. **AssemblyAI API**: Used to transcribe audio from YouTube videos.

   - [AssemblyAI API Documentation](https://www.assemblyai.com/docs/)

Make sure to obtain API keys for these services and add them to your `.env` file as shown in the installation instructions.

## Installation

1. Clone the repository:

   ```sh
   git clone <repository-url>
   cd backend/ai_blog_app
   ```

2. Create and activate a virtual environment:

   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the dependencies:

   ```sh
   pip install -r requirements.txt
   ```

4. Set up the environment variables:

   - Create a `.env` file in the `ai_blog_app` directory and add the following variables:
     ```
     =<SECRET_KEYyour-secret-key>
     DB_NAME=<your-database-name>
     DB_USER=<your-database-user>
     DB_PASSWORD=<your-database-password>
     DB_HOST=<your-database-host>
     DB_PORT=<your-database-port>
     OPENAI_API_KEY=<your-openai-api-key>
     ASSEMBLYAI_API_KEY=<your-assemblyai-api-key>
     ```

5. Apply the migrations:

   ```sh
   python [manage.py](http://_vscodecontentref_/18) migrate
   ```

6. Create a superuser:

   ```sh
   python [manage.py](http://_vscodecontentref_/19) createsuperuser
   ```

7. Run the development server:

   ```sh
   python [manage.py](http://_vscodecontentref_/20) runserver
   ```

8. Open your browser and go to `http://127.0.0.1:8000/` to access the application.

## Usage

- **Login/Signup**: Create an account or log in to access the blog generator.
- **Generate Blog**: Enter a YouTube video link and click the "Generate" button to create a blog article.
- **View Blogs**: View all generated blog articles and their details.
