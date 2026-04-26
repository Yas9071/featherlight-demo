<!DOCTYPE html>

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Featherlight Plugin Demo</title>

```
<!-- Featherlight CSS -->
<link href="https://cdn.jsdelivr.net/npm/featherlight@1.7.14/release/featherlight.min.css" rel="stylesheet">

<style>
    body {
        font-family: Arial, sans-serif;
        margin: 0;
        padding: 0;
        background: #fafafa;
    }

    .container {
        max-width: 1100px;
        margin: auto;
        padding: 40px;
    }

    h1 {
        text-align: center;
    }

    .subtitle {
        text-align: center;
        color: #666;
        margin-bottom: 30px;
    }

    .gallery {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 20px;
    }

    .gallery-item {
        position: relative;
        overflow: hidden;
        border-radius: 8px;
    }

    .gallery-item img {
        width: 100%;
        display: block;
    }

    .overlay {
        position: absolute;
        inset: 0;
        background: rgba(0,0,0,0.6);
        display: flex;
        justify-content: center;
        align-items: center;
        opacity: 0;
        transition: 0.3s;
    }

    .gallery-item:hover .overlay {
        opacity: 1;
    }

    .overlay span {
        color: white;
        font-weight: bold;
    }

    .rationale {
        margin-top: 50px;
        background: #f0f0f0;
        padding: 25px;
        border-radius: 8px;
    }
</style>
```

</head>

<body>

<div class="container">
    <h1>Featherlight.js Demo</h1>
    <p class="subtitle">JavaScript Lightbox Plugin Proof-of-Concept</p>

```
<div class="gallery">

    <div class="gallery-item">
        <a href="https://images.unsplash.com/photo-1506905925346-21bda4d32df4?w=1200" data-featherlight="image">
            <img src="https://images.unsplash.com/photo-1506905925346-21bda4d32df4?w=400">
            <div class="overlay"><span>Mountain</span></div>
        </a>
    </div>

    <div class="gallery-item">
        <a href="https://images.unsplash.com/photo-1470071459604-3b5ec3a7fe05?w=1200" data-featherlight="image">
            <img src="https://images.unsplash.com/photo-1470071459604-3b5ec3a7fe05?w=400">
            <div class="overlay"><span>Waterfall</span></div>
        </a>
    </div>

    <div class="gallery-item">
        <a href="https://images.unsplash.com/photo-1471922694854-711d2a195667?w=1200" data-featherlight="image">
            <img src="https://images.unsplash.com/photo-1471922694854-711d2a195667?w=400">
            <div class="overlay"><span>Cliff</span></div>
        </a>
    </div>

</div>

<div class="rationale">
    <h2>Design Rationale</h2>
    <p>
        This project uses the Featherlight.js plugin to demonstrate a lightbox effect. When a user clicks an image, it opens in a larger view without leaving the page.
    </p>
    <p>
        The benefit of this plugin is that it improves user experience by keeping interactions smooth and simple while requiring minimal code.
    </p>
    <p>
        This concept can be expanded into portfolios, product pages, or photography websites with added features like captions or filters.
    </p>
</div>
```

</div>

<!-- Required Scripts -->

<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>

<script src="https://cdn.jsdelivr.net/npm/featherlight@1.7.14/release/featherlight.min.js"></script>

</body>
</html>
