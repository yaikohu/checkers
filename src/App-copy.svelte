<!-- <script lang="ts">
	// import Square from "./Square.svelte";
	import type { Square as SquareT, Row, Board, Pawn } from "./interfaces/checkers";

	// Applying DRY principle;
	function createSquare(clr: string): SquareT {
		let coloredSqr: SquareT;
		coloredSqr = {
			color: clr,
			area: { width: "50px", height: "50px" },
			hasPawn: false,
		};
		return coloredSqr;
	}
	const sqrColors = ["beige", "black"]
	// let sqrs: {white: SquareT, black: SquareT};

	// for (const color in sqrColors) {
	// 	sqrs.white = createSquare(color)
	// }
	
	let whiteSquare: SquareT = createSquare("beige");
	let blackSquare: SquareT = createSquare("black");

	let pawnWhite: Pawn = {
		color: "beige",
		area: { width: "50px", height: "50px" },
	};

	let pawnBlack: Pawn = {
		color: "black",
		area: { width: "50px", height: "50px" },
	};
	// TODO: Create Square-objects with pawns
	// TODO: Implement a function that adds a square based on the Row.length property
	// TODO: Implement a function that allows you to select a row variation (start with black / start with white)
	let row_var1: Row = {
		squares: [
			whiteSquare,
			blackSquare,
			whiteSquare,
			blackSquare,
			whiteSquare,
			blackSquare,
			whiteSquare,
			blackSquare,
		],
		length: 8,
	};

	let row_var2: Row = {
		squares: [
			blackSquare,
			whiteSquare,
			blackSquare,
			whiteSquare,
			blackSquare,
			whiteSquare,
			blackSquare,
			whiteSquare,
		],
		length: 8,
	};
	// TODO: Implement a function that adds Board.width amount of rows to Board.rows
	let CheckersBoard: Board = {
		rows: [
			row_var1,
			row_var2,
			row_var1,
			row_var2,
			row_var1,
			row_var2,
			row_var1,
			row_var2,
		],
		width: 8,
	};

	// TODO: Add interactivity for playing checkers
</script>

<main>
	<div class="container">
		<div class="checkersboard">
			{#each CheckersBoard.rows as row}
				<div class="row">
					{#each row.squares as square}
						<div
							class="square"
							style="
									width: {square.area.width}; 
									height: {square.area.height}; 
									background-color: {square.color};"
						/>
					{/each}
				</div>
			{/each}
		</div>
	</div>
</main>

<style>
	.container {
		padding: 50px;
		display: flex;
		justify-content: center;
	}
	.checkersboard {
		display: flex;
		position: fixed;
		border: 1px solid black;
		/* eight squares times their width or length: 8 * 50px = 400px */
		max-width: 400px;
		max-height: 400px;
	}
</style> -->
