<script>
	/** @type {import('./$types').PageData} */
	export let data;
</script>

<div class="container flex flex-col justify-center items-center my-4 w-full h-fit">
	<section class="card p-2 w-[95%]">
		<h1 class="h1 text-center p-2">Sistemas gestores de bases de datos</h1>
		<p class="text-xl p-2">
			Los sistemas gestores de bases de datos (SGBD) son programas de software que permiten a los
			usuarios crear y mantener bases de datos. Estos sistemas proporcionan una interfaz para que
			los usuarios puedan insertar, actualizar, eliminar y recuperar datos de manera eficiente. Los
			SGBD también gestionan la seguridad de los datos, la integridad de la base de datos y la
			concurrencia, lo que permite a varios usuarios acceder y modificar la base de datos al mismo
			tiempo sin que se produzcan conflictos.
		</p>
		<p class="text-xl p-2">
			Además, los SGBD ofrecen capacidades de respaldo y recuperación que permiten a los usuarios
			restaurar la base de datos en caso de fallo del sistema o pérdida de datos. Algunos ejemplos
			de SGBD populares incluyen MySQL, PostgreSQL, SQLite, Oracle y Microsoft SQL Server. Estos
			sistemas son fundamentales para el almacenamiento y gestión de datos en una amplia gama de
			aplicaciones, desde sitios web y aplicaciones empresariales hasta sistemas embebidos y
			dispositivos móviles.
		</p>
		<div class="flex justify-center items-center p-2">
			<img src="/db-server-03.png" alt="SGBD" class="h-auto w-2/4 rounded-xl" />
		</div>
		<h3 class="h3 p-2">Ejemplos:</h3>
		<ul class="list [&>li]:p-2 [&>li]:text-xl">
			<li>
                <span>•</span>
                <span>
				MariaDB: MariaDB es un sistema gestor de bases de datos relacional de código abierto que se
				deriva de MySQL. Fue desarrollado por los creadores originales de MySQL y está diseñado como
				una alternativa compatible con MySQL, con mejoras y nuevas características. MariaDB se
				centra en la escalabilidad, la seguridad y el rendimiento, y es ampliamente utilizado en
				aplicaciones web y empresariales.
                </span>
			</li>
			<li>
                <span>•</span>
                <span>
				PostgreSQL: PostgreSQL es un sistema gestor de bases de datos relacional de código abierto
				que se destaca por su robustez, confiabilidad y capacidad de gestión de datos complejos.
				Ofrece un amplio conjunto de características avanzadas, incluyendo soporte para tipos de
				datos personalizados, consultas complejas, transacciones ACID, y replicación. PostgreSQL es
				conocido por su capacidad de escalabilidad y su énfasis en la conformidad con los
				estándares.
                </span>
			</li>
			<li>
                <span>•</span>
                <span>
				MySQL: MySQL es un sistema gestor de bases de datos relacional de código abierto que es
				ampliamente utilizado en aplicaciones web y empresariales. Es conocido por su velocidad,
				facilidad de uso y capacidad de escalabilidad. MySQL es una opción popular para aplicaciones
				que requieren una base de datos de alto rendimiento, como sitios web de comercio
				electrónico, blogs y aplicaciones de redes sociales.
                </span>
			</li>
		</ul>
	</section>
</div>
