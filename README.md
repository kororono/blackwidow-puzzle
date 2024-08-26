<!DOCTYPE html>
<html>
<head>
    <title>Black Widow 8808 Puzzle</title>
    <style>
        #puzzle-grid {
            display: grid;
            grid-template-columns: repeat(4, 100px);
            grid-template-rows: repeat(4, 100px);
            gap: 10px;
        }

        .tile {
            width: 100px;
            height: 100px;
            background-color: #333;
            border: 1px solid #666;
            cursor: pointer;
        }

        .revealed {
            background-image: url('black-widow-image.jpg'); /* Replace with your image */
            background-size: cover;
        }
    </style>
</head>
<body>
    <div id="puzzle-grid"></div>
    <script>
        const grid = document.getElementById('puzzle-grid');
        const characters = ['B', 'L', 'A', 'C', 'K', 'W', 'I', 'D', 'O', 'W', '8', '8', '0', '8'];

        function createPuzzle() {
            characters.sort(() => Math.random() - 0.5);

            for (let i = 0; i < characters.length; i++) {
                const tile = document.createElement('div');
                tile.classList.add('tile');
                tile.textContent = characters[i];
                tile.setAttribute('data-character', characters[i]);
                tile.addEventListener('click', flipTile);
                grid.appendChild(tile);
            }
        }

        function flipTile() {
            if (!this.classList.contains('revealed')) {
                this.classList.add('revealed');
            }
        }

        createPuzzle();
    </script>
</body>
</html><!DOCTYPE html>
<html>
<head>
    <title>Black Widow 8808 Puzzle</title>
    <style>
        #puzzle-grid {
            display: grid;
            grid-template-columns: repeat(4, 100px);
            grid-template-rows: repeat(4, 100px);
            gap: 10px;
        }

        .tile {
            width: 100px;
            height: 100px;
            background-color: #333;
            border: 1px solid #666;
            cursor: pointer;
        }

        .revealed {
            background-image: url('black-widow-image.jpg'); /* Replace with your image */
            background-size: cover;
        }
    </style>
</head>
<body>
    <div id="puzzle-grid"></div>
    <script>
        const grid = document.getElementById('puzzle-grid');
        const characters = ['B', 'L', 'A', 'C', 'K', 'W', 'I', 'D', 'O', 'W', '8', '8', '0', '8'];

        function createPuzzle() {
            characters.sort(() => Math.random() - 0.5);

            for (let i = 0; i < characters.length; i++) {
                const tile = document.createElement('div');
                tile.classList.add('tile');
                tile.textContent = characters[i];
                tile.setAttribute('data-character', characters[i]);
                tile.addEventListener('click', flipTile);
                grid.appendChild(tile);
            }
        }

        function flipTile() {
            if (!this.classList.contains('revealed')) {
                this.classList.add('revealed');
            }
        }

        createPuzzle();
    </script>
</body>
</html>
