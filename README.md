# index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Poetry Website</title>
    <link rel="stylesheet" href="styles.css">
    <script>
        function toggleLike(likeButton) {
            likeButton.classList.toggle('liked');
            if (likeButton.classList.contains('liked')) {
                likeButton.innerHTML = "Liked";
            } else {
                likeButton.innerHTML = "Like";
            }
        }
    </script>
</head>
<body>

    <!-- Header Section -->
    <header>
        <h1>Welcome to My Poetry</h1>
        <p>Explore the world through poetry. Feel the emotion with every verse.</p>
    </header>

    <!-- Navigation Bar -->
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#poetry">Poetry</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Poetry Section -->
    <section class="poetry-box">
        <div class="poetry-post">
            <h2>Sanwal Poetry</h2>
            <p class="poem-content">This is a sample poem in English, styled with a black theme. Visitors can like and comment on it.</p>
            <div class="poetry-actions">
                <button class="like-btn" onclick="toggleLike(this)">Like</button>
                <button class="comment-btn">Comment</button>
            </div>
            <div class="comments-section">
                <input type="text" placeholder="Add a comment...">
                <button class="submit-comment">Submit</button>
            </div>
        </div>
    </section>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2025 My Poetry Website | <a href="mailto:contact@poetry.com">Contact Us</a></p>
    </footer>

</body>
</html>
