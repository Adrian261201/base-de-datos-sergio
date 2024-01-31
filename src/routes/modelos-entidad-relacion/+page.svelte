<script>
	/** @type {import('./$types').PageData} */
	export let data;
</script>

<svelte:head><title>Modelos de Entidad Relación</title></svelte:head>

<div class="container flex justify-center items-center my-4 w-full h-fit">
	<section class="card p-2 w-[95%]">
		<h1 class="h1 text-center p-2">Modelos de Entidad Relación</h1>
		<p class="text-xl p-2">
			Un modelo entidad-relación (ER) es un enfoque para diseñar bases de datos que representa la
			información y las reglas que gobiernan su estructura. En un modelo ER, las entidades son
			objetos del mundo real o conceptos abstractos, como personas, lugares, cosas, eventos, o
			conceptos. Estas entidades se representan en la base de datos como tablas. Los atributos, por
			otro lado, son las propiedades o características de las entidades, como el nombre, la edad, el
			color, etc.
		</p>
		<p class="text-xl p-2">
			El modelo entidad-relación también describe las relaciones entre las entidades. Las relaciones
			representan cómo las entidades están conectadas entre sí. Por ejemplo, una relación puede ser
			"trabaja para", que conecta a un empleado con la empresa para la que trabaja. Las direcciones
			en un modelo ER se refieren a la forma en que las relaciones y atributos se organizan y se
			conectan entre sí, lo que ayuda a definir la estructura de la base de datos y cómo se accede a
			la información.
		</p>
		<div class="flex justify-center items-center p-2">
			<img src="/modelo-er.png" alt="Modelo ER" class="h-auto w-2/3 rounded-xl" />
		</div>
		<h2 class="h2 text-center p-2">Características</h2>
		<p class="text-xl p-2">
			Los elementos de un modelo ER son las entidades, los atributos y las relaciones.
		</p>
		<ul class="list [&>li]:p-2 [&>li]:text-xl">
			<li>
				<span>•</span>
				<span>
					Entidad: es un objeto del mundo real o un concepto abstracto que se representa en la base
					de datos. Por ejemplo, en una base de datos de una empresa, las entidades pueden ser
					"cliente", "producto", "empleado", etc. Cada entidad se representa como una tabla en la
					base de datos.
				</span>
			</li>
			<li>
				<span>•</span>
				<span>
					Atributo: son las propiedades o características de las entidades. Por ejemplo, para la
					entidad "cliente", los atributos pueden ser el nombre, la dirección, el número de
					teléfono, etc. Los atributos se representan como columnas en la tabla de la entidad.
				</span>
			</li>
			<li>
				<span>•</span>
				<span>
					Relación: representan cómo las entidades están conectadas entre sí. Por ejemplo, en una
					base de datos de una universidad, puede haber una relación entre las entidades
					"estudiante" y "curso" que indica qué estudiantes están inscritos en qué cursos.
				</span>
			</li>
		</ul>
		<h2 class="h2 text-center p-2">Correspondencia cardinal</h2>
		<p class="text-xl p-2">
			La correspondencia cardinal en un modelo entidad-relación (ER) describe la cantidad de
			instancias de una entidad que pueden estar asociadas con la cantidad de instancias de otra
			entidad a través de una relación. Hay tres tipos principales de correspondencia cardinal:
		</p>
		<ul class="list [&>li]:p-2 [&>li]:text-xl">
			<li>
				<span>•</span>
				<span>
					Uno a uno (1:1): Indica que una instancia de una entidad solo puede estar asociada con una
					instancia de otra entidad, y viceversa. Por ejemplo, un pasaporte está asociado a una
					persona y una persona tiene un solo pasaporte.
				</span>
			</li>
			<li>
				<span>•</span>
				<span>
					Uno a muchos (1:N): Indica que una instancia de una entidad puede estar asociada con una o
					más instancias de otra entidad, pero una instancia de la otra entidad solo puede estar
					asociada con una instancia de la primera entidad. Por ejemplo, un cliente puede realizar
					muchas compras, pero cada compra está asociada a un solo cliente.
				</span>
			</li>
			<li>
				<span>•</span>
				<span>
					Muchos a muchos (M:N): Indica que una instancia de una entidad puede estar asociada con
					muchas instancias de otra entidad, y viceversa. Por ejemplo, un estudiante puede
					inscribirse en múltiples cursos, y un curso puede tener varios estudiantes inscritos.
				</span>
			</li>
		</ul>
		<div class="flex flex-row-reverse justify-between items-center p-2">
			<a href="/normalizaciones" class="btn variant-filled font-bold"
				>Normalización<svg
					xmlns="http://www.w3.org/2000/svg"
					class="icon icon-tabler icon-tabler-arrow-narrow-right"
					width="24"
					height="24"
					viewBox="0 0 24 24"
					stroke-width="2"
					stroke="currentColor"
					fill="none"
					stroke-linecap="round"
					stroke-linejoin="round"
					><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path d="M5 12l14 0" /><path
						d="M15 16l4 -4"
					/><path d="M15 8l4 4" /></svg
				></a
			>
			<a href="/sistemas-gestores" class="btn variant-filled font-bold"
				><svg
					xmlns="http://www.w3.org/2000/svg"
					class="icon icon-tabler icon-tabler-arrow-narrow-left"
					width="24"
					height="24"
					viewBox="0 0 24 24"
					stroke-width="2"
					stroke="currentColor"
					fill="none"
					stroke-linecap="round"
					stroke-linejoin="round"
					><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path d="M5 12l14 0" /><path
						d="M5 12l4 4"
					/><path d="M5 12l4 -4" /></svg
				>Sistemas gestores</a
			>
		</div>
	</section>
</div>
