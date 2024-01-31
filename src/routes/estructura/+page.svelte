<script>
	/** @type {import('./$types').PageData} */
	export let data;
</script>

<svelte:head><title>Estructura</title></svelte:head>

<div class="container flex justify-center items-center my-4 w-full h-fit">
	<section class="card p-2 w-[95%]">
		<h1 class="h1 text-center p-2">Estructura</h1>
		<p class="text-xl p-2">
			Tabla: Una tabla en una base de datos relacional es una estructura que organiza los datos en
			filas y columnas. Cada fila representa una entidad única y cada columna representa un atributo
			de esa entidad. Las tablas se utilizan para almacenar y organizar los datos de manera
			estructurada, y se pueden relacionar entre sí mediante claves primarias y claves foráneas para
			representar relaciones entre entidades.
		</p>
		<p class="text-xl p-2">
			Campo: Un campo en una base de datos se refiere a una columna individual en una tabla. Cada
			campo representa un atributo específico de la entidad que se está modelando. Por ejemplo, en
			una tabla de "empleados", los campos podrían incluir "nombre", "apellido", "edad", "cargo",
			etc. Cada campo tiene un nombre único dentro de la tabla y define el tipo de datos que puede
			almacenar, como texto, número, fecha, etc.
		</p>
		<p class="text-xl p-2">
			Registro: Un registro en una base de datos se refiere a una fila individual en una tabla. Cada
			registro representa una instancia única de la entidad que está siendo modelada. Por ejemplo,
			en una tabla de "empleados", cada registro representaría a un empleado específico, con sus
			atributos como nombre, apellido, edad, cargo, etc. Los registros contienen los valores de los
			campos que representan las características específicas de la entidad.
		</p>
        <div class="flex justify-center items-center p-2">
            <img src="/OIG2.png" alt="" class="h-auto w-1/4 rounded-xl">
        </div>
	</section>
</div>
