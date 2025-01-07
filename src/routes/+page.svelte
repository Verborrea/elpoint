<script>
	import { ArrowLeft, UserRound, KeyRound } from 'lucide-svelte';
</script>

<main>
	<header>
		<a href="/" class="return">
			<ArrowLeft />
			Regresar
		</a>
	</header>
	<img src="https://upload.wikimedia.org/wikipedia/commons/f/f4/Pueblo_de_Macondo.jpg" alt="Macondo">
	<h1>Extracto de Cien Años de Soledad</h1>
	<h2>Gabriel García Márquez</h2>
	<h3>Lun 6 ene.</h3>
	<p>
		En un lugar de <strong>Macondo</strong>, <em>cuyo nombre cambiaría con los años</em>, José Arcadio
		Buendía y Úrsula Iguarán fundaron una dinastía condenada a cien años de
		soledad. Los Buendía, con su <a href="/">pasión desbordante</a>, sus amores prohibidos y sus
		sueños imposibles, fueron testigos de guerras, milagros y desastres.
	</p>
	<p>
		Macondo, que nació como un <q>sueño de prosperidad</q>, se convirtió en el
		escenario de una historia cíclica, donde los mismos errores, nombres y
		pasiones se repetían como un eco inagotable del destino.
	</p>
	<p>Gracias por leer. Deje sus comentarios.</p>
	<label for="name">
		<span>Nombre Completo:</span>
		<div class="container">
			<UserRound />
			<input type="text" name="name" id="name" placeholder="Jose Arcadio Buendía">
		</div>
	</label>
	<label for="password">
		<span>Contraseña:</span>
		<div class="container">
			<KeyRound />
			<input type="password" name="password" id="password" placeholder="••••••••••">
		</div>
	</label>
	<button type="button">Botón principal</button>
	<button type="button" class="btn-secondary">Botón secundario</button>
</main>
<footer>
	<p>&copy; 2025 elPoint</p>
</footer>

<style>
	.return {
		display: flex;
		align-items: center;
		gap: 8px;
		text-decoration: none;
		color: var(--tx2);
	}
	main {
		padding: 32px 24px;
		display: flex;
		flex-direction: column;
		gap: 16px;
	}
	footer {
		padding: 32px 24px;
		text-align: center;
	}
</style>