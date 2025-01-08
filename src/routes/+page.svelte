<script>
	import Categories from "./Categories.svelte"
	import { ArrowLeft, UserRound, KeyRound } from "lucide-svelte";
</script>

<main class="fcol g16">
	<header>
		<a href="/" class="return fc">
			<ArrowLeft />
			Regresar
		</a>
	</header>
	<img
		src="https://upload.wikimedia.org/wikipedia/commons/f/f4/Pueblo_de_Macondo.jpg"
		alt="Macondo"
	/>
	<h1>Extracto de Cien Años de Soledad</h1>
	<h2>Gabriel García Márquez</h2>
	<h3>Lun 6 ene.</h3>
	<Categories/>
	<p>
		En un lugar de <strong>Macondo</strong>,
		<em>cuyo nombre cambiaría con los años</em>, José Arcadio Buendía y Úrsula
		Iguarán fundaron una dinastía condenada a cien años de soledad. Los Buendía,
		con su <a href="/">pasión desbordante</a>, sus amores prohibidos y sus
		sueños imposibles, fueron testigos de guerras, milagros y desastres.
	</p>
	<p>
		Macondo, que nació como un <q>sueño de prosperidad</q>, se convirtió en el
		escenario de una historia cíclica, donde los mismos errores, nombres y
		pasiones se repetían como un eco inagotable del destino.
	</p>
	<p>Gracias por leer. Deje sus comentarios.</p>
	<form method="get" class="fcol g16">
		<h2>Formulario:</h2>
		<label for="name">
			<span>Nombre Completo:</span>
			<div class="container">
				<UserRound size={16} absoluteStrokeWidth />
				<input
					type="text"
					name="name"
					id="name"
					placeholder="Juan Pérez"
					pattern="^[A-Za-zÁÉÍÓÚáéíóúÑñ\s]+$"
				/>
			</div>
		</label>
		<label for="address">
			<span>Dirección:</span>
			<div class="container">
				<input
					type="text"
					name="address"
					id="address"
					placeholder="El parque del avión"
					pattern="^[A-Za-zÁÉÍÓÚáéíóúÑñ\s]+$"
				/>
			</div>
		</label>
		<div class="btns fc g16">
			<button type="submit">Enviar</button>
			<button type="reset" class="btn-secondary">Borrar</button>
		</div>
	</form>
</main>
<footer>
	<p>&copy; 2025 elPoint</p>
</footer>

<style>
	.return {
		gap: 8px;
		text-decoration: none;
		color: var(--tx2);
	}
	main {
		margin: auto;
		max-width: 700px;

		padding: 32px 24px;
	}
	footer {
		padding: 0px 24px 32px;
		text-align: center;
	}
	.btns button {
		width: 100%;
	}
</style>
