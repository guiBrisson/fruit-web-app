<script>
	const monthlyFruits = [
		{
			month: 'janeiro',
			fruits:
				'Abacaxi, carambola, coco-verde, figo, fruta-do-conde, laranja-pera, mamão, maracujá, melancia, nectarina'
		},
		{
			month: 'fevereiro',
			fruits:
				'Abacate, ameixa, carambola, figo, pinha (conhecida em algumas regiões por fruta-do--conde), goiaba, jaca, maçã, pera'
		},
		{
			month: 'março',
			fruits:
				'Abacate, abacaxi, ameixa, banana-maçã, banana-nanica, goiaba, jaca, limão, maçã, pera'
		},
		{
			month: 'abril',
			fruits: 'Abacate, banana-maçã, caqui, jaca, kiwi, maçã, pera'
		},
		{
			month: 'maio',
			fruits: 'Abacate, banana-maçã, caqui, kiwi, jaca, maçã, pera, tangerina'
		},
		{
			month: 'junho',
			fruits: 'Carambola, kiwi,laranja-lima, tangerina (ou mexerica)'
		},
		{
			month: 'junlho',
			fruits: 'Carambola, kiwi, laranja-lima, tangerina(ou mexerica)'
		},
		{
			month: 'agosto',
			fruits: 'Caju, carambola, laranja-pera, lima, maçã,tangerina(ou mexerica), morango'
		},
		{
			month: 'setembro',
			fruits: 'Abacaxi, banana-nanica, caju, jabuticaba, laranja-lima, laranja-pera, mexerica'
		},
		{
			month: 'outubro',
			fruits: 'Abacaxi, acerola, banana-nanica, banana-prata, caju, manga, jabuticaba, lima'
		},
		{
			month: 'novembro',
			fruits:
				' Abacaxi, acerola, banana-nanica, banana-prata, caju, coco-verde, mamão, manga, melancia, melão, pêssego'
		},
		{
			month: 'dezembro',
			fruits: 'Ameixa, cereja, damasco, figo, lichia, manga, melancia, melão, nectarina'
		}
	];
</script>

<div class="flex flex-col justify-center">
	<section class="">
		<div class="mx-auto max-w-screen-2xl px-4 py-48 lg:flex lg:items-center">
			<div class="mx-auto max-w-2xl text-center">
				<h1 class="text-3xl font-extrabold sm:text-5xl">
					MAIS FRUTAS
					<strong class="font-extrabold text-primary sm:block"> TODO DIA </strong>
				</h1>

				<p class="mt-4 sm:text-xl sm:leading-relaxed">
					Aproveite a riqueza das feiras livres e aposte nas frutas da estação para garantir tudo o
					que elas podem oferecer para o seu organismo.
				</p>
			</div>
		</div>
	</section>

	<section class="bg-gray-50">
		<div class="mx-auto max-w-screen-xl px-4 py-16 sm:px-6 sm:py-24 lg:px-8">
			<h1 class="text-2xl font-semibold text-gray-800 capitalize lg:text-3xl">
				safra de <span class="underline decoration-primary">frutas</span>
			</h1>

			<p class="mt-4 text-gray-500 font-medium max-w-xl ">
				A melhor maneira de colocar mais nutrientes no cardápio é aproveitando o período de safra,
				onde os alimentos não precisam de pesticidas para crescer com saúde.
			</p>
			<div
				class="grid grid-cols-1 gap-x-12 gap-y-8 mx:gap-x-8 mt-8 xl:mt-12 md:grid-cols-2 xl:grid-cols-3 items-center mx-auto md:text-center items-stretch"
			>
				{#each monthlyFruits as month}
					<div class="md:space-y-3 space-y-1 md:border md:border-primary md:rounded-xl min-h-max md:p-6 md:hover:shadow-lg hover:cursor-pointer">
						<h1 class="text-xl font-semibold text-primary capitalize ">{month.month}</h1>

						<p class="">{month.fruits}</p>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<section class="bg-white">
		<div class="mx-auto max-w-screen-xl px-4 py-16 sm:px-6 sm:py-24 lg:px-8">
			<div class="mt-8 grid grid-cols-1 gap-8 lg:grid-cols-2 lg:gap-16">
				<div class="relative h-64 overflow-hidden sm:h-80 lg:h-full">
					<img
						alt=""
						src="https://images.unsplash.com/photo-1598512752423-099d75d4865c?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1470&q=80"
						class="absolute inset-0 h-full w-full object-cover"
					/>
				</div>

				<div class="lg:py-4">
					<article class="text-gray-600">
						<h2 class="text-3xl font-bold sm:text-4xl mb-8">Neutralize os agrotóxicos</h2>
						<p>
							Nem sempre é possível comprar alimentos sem agrotóxico. Mas dá para neutralizá-los. De
							acordo com agentes da vigilância sanitária, colocar os alimentos de molho no
							bicarbonato de sódio é o melhor a se fazer. A nutricionista Sonja Salles ensina como:
						</p>
						<p class="mt-6 mb-2 text-primary font-bold">INGREDIENTES:</p>
						<p>
							<li>1 colher de sopa de bicarbonato de sódio</li>
							<li>1 litro de água limpa e potável</li>
						</p>
						<p class="mt-4 mb-2 text-primary font-bold">MODO DE PREPARO:</p>
						<p>
							Coloque o alimento, depois de higienizado, de molho nessa mistura por pelo menos 15
							minutos. "Quimicamente essa fórmula caseira consegue neutralizar os agrotóxicos,
							diminuindo significativamente os impactos deles no organismo", explica.
						</p>
					</article>
				</div>
			</div>
		</div>
	</section>
</div>
