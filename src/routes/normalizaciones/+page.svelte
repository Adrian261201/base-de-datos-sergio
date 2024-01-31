<script>
	/** @type {import('./$types').PageData} */
	export let data;
</script>

<svelte:head><title>Normalizaciones</title></svelte:head>

<div class="container flex justify-center items-center my-4 w-full h-fit">
	<section class="card p-2 w-[95%]">
		<h1 class="h1 text-center p-2">Descripción de la normalización</h1>
		<p class="text-xl p-2">
			La normalización es el proceso de organizar los datos de una base de datos. Se incluye la
			creación de tablas y el establecimiento de relaciones entre ellas según reglas diseñadas tanto
			para proteger los datos como para hacer que la base de datos sea más flexible al eliminar la
			redundancia y las dependencias incoherentes.
		</p>
		<p class="text-xl p-2">
			Los datos redundantes desperdician el espacio de disco y crean problemas de mantenimiento. Si
			hay que cambiar datos que existen en más de un lugar, se deben cambiar de la misma forma
			exactamente en todas sus ubicaciones. Un cambio en la dirección de un cliente es mucho más
			fácil de implementar si los datos sólo se almacenan en la tabla Clientes y no en algún otro
			lugar de la base de datos.
		</p>
		<div class="flex justify-center items-center p-2" />
		<img src="/normalizacion.png" alt="" class="h-auto w-2/4 rounded-xl mx-auto" />
		<div />
		<h2 class="h2 text-center p-2">Primera forma normal</h2>
		<ul class="list [&>li]:p-2 [&>li]:text-xl">
			<li>
				<span>•</span>
				<span>Elimine los grupos repetidos de las tablas individuales.</span>
			</li>
			<li>
				<span>•</span>
				<span>Cree una tabla independiente para cada conjunto de datos relacionados.</span>
			</li>
			<li>
				<span>•</span>
				<span>Identifique cada conjunto de datos relacionados con una clave principal.</span>
			</li>
		</ul>
		<p class="text-xl p-2">
			No use varios campos en una misma tabla para almacenar datos similares. Por ejemplo, para
			realizar el seguimiento de un elemento del inventario que proviene de dos orígenes posibles,
			un registro del inventario puede contener campos para el Código de proveedor 1 y para el
			Código de proveedor 2.
		</p>
		<p class="text-xl p-2">
			¿Qué ocurre cuando se agrega un tercer proveedor? Agregar un campo no es la respuesta;
			requiere modificaciones del programa y de la tabla y no se adapta sin problemas a un número
			dinámico de proveedores. En su lugar, coloque toda la información de los proveedores en una
			tabla independiente denominada Proveedores y después vincule el inventario a los proveedores
			con el número de elemento como clave, o los proveedores al inventario con el código de
			proveedor como clave.
		</p>
		<h2 class="h2 text-center p-2">Segunda forma normal</h2>
		<ul class="list [&>li]:p-2 [&>li]:text-xl">
			<li>
				<span>•</span>
				<span>
					Cree tablas independientes para conjuntos de valores que se apliquen a varios registros.
				</span>
			</li>
			<li>
				<span>•</span>
				<span>Relacione estas tablas con una clave externa.</span>
			</li>
		</ul>
		<p class="text-xl p-2">
			Los registros no deben depender de nada más que de la clave principal de una tabla (una clave
			compuesta, si es necesario). Por ejemplo, considere la dirección de un cliente en un sistema
			de contabilidad. La dirección se necesita en la tabla Clientes, pero también en las tablas
			Pedidos, Envíos, Facturas, Cuentas por cobrar y Colecciones. En lugar de almacenar la
			dirección de un cliente como una entrada independiente en cada una de estas tablas, almacénela
			en un lugar, ya sea en la tabla Clientes o en una tabla Direcciones independiente.
		</p>
		<div class="flex justify-center items-center p-2">
			<img src="mona-china-c++.jpg" alt="" class="h-auto w-2/4 rounded-xl" />
		</div>
		<h2 class="h2 text-center p-2">Tercera forma normal</h2>
		<ul class="list [&>li]:p-2 [&>li]:text-xl">
			<li>
				<span>•</span>
				<span>Eliminar los campos que no dependen de la clave.</span>
			</li>
		</ul>
		<p class="text-xl p-2">
			Los valores de un registro que no forman parte de la clave de ese registro no pertenecen a la
			tabla. En general, siempre que el contenido de un grupo de campos pueda aplicarse a más de un
			único registro de la tabla, considere colocar estos campos en una tabla independiente.
		</p>
		<p class="text-xl p-2">
			Por ejemplo, en una tabla Contratación de empleados, puede incluirse el nombre de la
			universidad y la dirección de un candidato. Pero necesita una lista completa de universidades
			para enviar mensajes de correo electrónico en grupo. Si la información de las universidades se
			almacena en la tabla Candidatos, no hay forma de enumerar las universidades que no tengan
			candidatos en ese momento. Cree una tabla Universidades independiente y vincúlela a la tabla
			Candidatos con el código de universidad como clave.
		</p>
		<p class="text-xl p-2">
			EXCEPCIÓN: cumplir la tercera forma normal, aunque en teoría es deseable, no siempre es
			práctico. Si tiene una tabla Clientes y desea eliminar todas las dependencias posibles entre
			los campos, debe crear tablas independientes para las ciudades, códigos postales,
			representantes de venta, clases de clientes y cualquier otro factor que pueda estar duplicado
			en varios registros. En teoría, la normalización merece la pena. Sin embargo, muchas tablas
			pequeñas pueden degradar el rendimiento o superar la capacidad de memoria o de archivos
			abiertos.
		</p>
	</section>
</div>
