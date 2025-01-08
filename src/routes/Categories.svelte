<script>
	import { Utensils, Heart, Martini, TreePine } from "lucide-svelte";
</script>

<nav>
	<div class="scrollable fc g8">
		<label for="todo">
			<input type="radio" name="category" id="todo" checked>
			<span>Todo</span>
		</label>
		<label for="comida">
			<input type="radio" name="category" id="comida">
			<span class="fc g8">
				<Utensils size={16} absoluteStrokeWidth />
				Comida
			</span>
		</label>
		<label for="amor">
			<input type="radio" name="category" id="amor">
			<span class="fc g8">
				<Heart size={16} absoluteStrokeWidth />
				Parejas
			</span>
		</label>
		<label for="noche">
			<input type="radio" name="category" id="noche">
			<span class="fc g8">
				<Martini size={16} absoluteStrokeWidth />
				Vida Nocturna
			</span>
		</label>
		<label for="chill">
			<input type="radio" name="category" id="chill">
			<span class="fc g8">
				<TreePine size={16} absoluteStrokeWidth />
				Chill
			</span>
		</label>
	</div>
	<div class="gradientl"></div>
	<div class="gradientr"></div>
</nav>

<style>
	nav {
		width: calc(100% + 48px);
    position: relative;
    left: -24px;
    right: -24px;
	}
	.gradientl, .gradientr {
		position: absolute;
		width: 24px;
		height: 100%;
		top: 0;
	}
	.gradientl {
		left: 0px;
		background: linear-gradient(90deg, var(--bg), transparent);
	}
	.gradientr {
		right: 0px;
		background: linear-gradient(90deg, transparent, var(--bg));
	}
	.scrollable {
    overflow-x: scroll;
    scrollbar-width: none;
    -ms-overflow-style: none;
    padding-inline: 24px;
	}
	.scrollable::-webkit-scrollbar {
    display: none;
	}
	input {
		display: none;
	}
	span {
		padding: 12px 16px;
		text-transform: uppercase;
		border-radius: 12px;
		background: var(--sec);
		font-weight: bold;
		white-space: nowrap;
	}
	input:checked+span {
		background: var(--tx1);
		color: var(--bg);
	}
</style>
