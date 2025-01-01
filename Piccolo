<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Social Platform</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
        }
        header {
            background-color: #4CAF50;
            color: white;
            padding: 1rem;
            text-align: center;
        }
        .container {
            width: 90%;
            max-width: 800px;
            margin: 2rem auto;
            background: white;
            padding: 1rem;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        .post {
            border-bottom: 1px solid #ddd;
            padding: 1rem 0;
        }
        .post:last-child {
            border-bottom: none;
        }
        .post h3 {
            margin: 0;
        }
        .post p {
            margin: 0.5rem 0 0;
        }
        .new-post {
            margin-bottom: 2rem;
        }
        .new-post textarea {
            width: 100%;
            padding: 0.5rem;
            font-size: 1rem;
            margin-bottom: 0.5rem;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        .new-post button {
            padding: 0.5rem 1rem;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        .new-post button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <header>
        <h1>Simple Social Platform</h1>
    </header>

    <div class="container">
        <div class="new-post">
            <h2>Create a New Post</h2>
            <textarea id="postContent" rows="3" placeholder="What's on your mind?"></textarea>
            <button onclick="addPost()">Post</button>
        </div>

        <div id="posts">
            <h2>Recent Posts</h2>
            <!-- Posts will appear here -->
        </div>
    </div>

    <script>
        const postsContainer = document.getElementById('posts');

        function addPost() {
            const postContent = document.getElementById('postContent').value;
            if (postContent.trim() === '') {
                alert('Post content cannot be empty!');
                return;
            }

            const postDiv = document.createElement('div');
            postDiv.className = 'post';

            const postTitle = document.createElement('h3');
            postTitle.textContent = 'New Post';
            
            const postText = document.createElement('p');
            postText.textContent = postContent;

            postDiv.appendChild(postTitle);
            postDiv.appendChild(postText);
            postsContainer.appendChild(postDiv);

            document.getElementById('postContent').value = '';
        }
    </script>
</body>
</html>
