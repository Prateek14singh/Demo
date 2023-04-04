<script>
	import '../../Design.css';
	import Data from '../../Data.json';
	// import * as te from 'tw-elements';
</script>

<nav class="bg-white sticky top-0 drop-shadow-md items-center">
	<div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8 flex justify-between py-4">
		<a href="./"
			><img
				src="data:image/png;base64,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"
				alt="DMART"
			/></a
		>

		<a class="text-black font-bold py-4 px-2 hover:bg-green-100 text-center" href="./About"
			>ABOUT US</a
		>
		<a class="text-black font-bold py-4 px-2 hover:bg-green-100 text-center" href="./Categories"
			>CATEGORIES</a
		>
		<a class="text-black font-bold py-4 px-2 hover:bg-green-100 text-center" href="/Social Outreach"
			>SOCIAL OUTREACH</a
		>
		<a
			class="text-black font-bold py-4 px-2 hover:bg-green-100 text-center"
			href="./Partner with us">PARTNER WITH US</a
		>
		<div class="text-black font-bold py-4 px-2 hover:bg-green-100 text-center">CAREERS</div>
		<div class="text-black font-bold py-4 px-2 hover:bg-green-100 text-center">FEEDBACK</div>
		<div class="flex justify-between text-lg font-bold py-4" />
	</div>
</nav>
<div class="font-bold underline underline-offset-4 justify-center flex my-4">PARTNER WITH US</div>
<ul
	class="m-5 flex list-none flex-col flex-wrap pl-0 md:flex-row"
	id="pills-tab"
	role="tablist"
	data-te-nav-ref
>
	<li role="presentation">
		<a
			href="./Partner with us"
			class="my-2 block rounded bg-neutral-100 px-7 pt-4 pb-3.5 text-xs font-medium uppercase leading-tight text-neutral-500 data-[te-nav-active]:!bg-green-400 data-[te-nav-active]:text-primary-700 dark:bg-green-700 dark:text-white dark:data-[te-nav-active]:text-white font-semibold md:mr-4"
			id="pills-home-tab"
			data-te-toggle="pill"
			data-te-target="#pills-home"
			data-te-nav-active
			role="tab"
			aria-controls="pills-home"
			aria-selected="true">SUPPLIER</a
		>
	</li>
	<li role="presentation">
		<a
			href="./Partner with us"
			class="my-2 block rounded bg-neutral-100 px-7 pt-4 pb-3.5 text-xs font-medium uppercase leading-tight text-neutral-500 data-[te-nav-active]:!bg-green-400 data-[te-nav-active]:text-primary-700 dark:bg-green-400 dark:text-white dark:data-[te-nav-active]:text-primary-700 md:mr-4"
			id="pills-profile-tab"
			data-te-toggle="pill"
			data-te-target="#pills-profile"
			role="tab"
			aria-controls="pills-profile"
			aria-selected="false">LANDLORDS</a
		>
	</li>
</ul>
<div class="mb-2">
	<div
		class="hidden opacity-0 opacity-100 transition-opacity duration-150 ease-linear data-[te-tab-active]:block"
		id="pills-home"
		role="tabpanel"
		aria-labelledby="pills-home-tab"
		data-te-tab-active
	>
		<div class="my-4 mx-8">
			<p class="mb-4">
				Do you have a quality product that needs an audience? We at DMart believe in joining hands
				with the right partners in order to provide high-quality yet affordable products to our
				customers. We invite suppliers to join us in our endeavour to offer the best to our
				customers. Be a part of our esteemed list of suppliers - with whom we have successful
				long-term partnerships - for a commercially satisfying and profitable relationship.
			</p>
			<p class="text-red-600 font-bold mb-4">
				We are temporarily suspending our "Tuesday Walk-ins" for all Vendors.
			</p>
			<p class="mb-4">
				You may continue to fill in the below form along with your product details. Our team will
				get in touch with you based on requirements.
			</p>
			<p class="mb-4">Fields marked with * are mandatory.</p>
			<div class="flex justify-between">
				<div class="w-1/2 p-4">
					<div class="font-bold underline underline-offset-4 my-4">Contact Details</div>
					{#each Data.partner as data}
						<div class="relative mb-3 xl:w-96 w-full" data-te-input-wrapper-init>
							<input
								type="text"
								class="peer block min-h-[auto] w-full rounded border-2 border-blue-400 bg-transparent py-[0.32rem] px-3 leading-[1.6] outline-solid transition-all duration-200 ease-linear focus:placeholder:opacity-100 data-[te-input-state-active]:placeholder:opacity-100 motion-reduce:transition-none dark:text-neutral-200 dark:placeholder:text-neutral-200 [&:not([data-te-input-placeholder-active])]:placeholder:opacity-0"
								id="exampleFormControlInput1"
								placeholder={data.placeholder}
							/>
							<label
								for="exampleFormControlInput1"
								class="pointer-events-none absolute top-0 left-3 mb-0 max-w-[90%] origin-[0_0] truncate pt-[0.37rem] leading-[1.6] text-neutral-500 transition-all duration-200 ease-out peer-focus:-translate-y-[0.9rem] peer-focus:scale-[0.8] peer-focus:text-primary peer-data-[te-input-state-active]:-translate-y-[0.9rem] peer-data-[te-input-state-active]:scale-[0.8] motion-reduce:transition-none dark:text-neutral-200 dark:peer-focus:text-neutral-200"
								>{data.title}
							</label>
						</div>
					{/each}
				</div>
				<div class="w-1/2 p-4">
					<div class="font-bold underline underline-offset-4 my-4">Product Details</div>
					{#each Data.product as data}
						<div class="relative mb-3 xl:w-96 w-full" data-te-input-wrapper-init>
							<input
								type="text"
								class="peer block min-h-[auto] w-full rounded border-2 border-blue-400 bg-transparent py-[0.32rem] px-3 leading-[1.6] outline-solid transition-all duration-200 ease-linear focus:placeholder:opacity-100 data-[te-input-state-active]:placeholder:opacity-100 motion-reduce:transition-none dark:text-neutral-200 dark:placeholder:text-neutral-200 [&:not([data-te-input-placeholder-active])]:placeholder:opacity-0"
								id="exampleFormControlInput1"
								placeholder={data.placeholder}
							/>
							<label
								for="exampleFormControlInput1"
								class="pointer-events-none absolute top-0 left-3 mb-0 max-w-[90%] origin-[0_0] truncate pt-[0.37rem] leading-[1.6] text-neutral-500 transition-all duration-200 ease-out peer-focus:-translate-y-[0.9rem] peer-focus:scale-[0.8] peer-focus:text-primary peer-data-[te-input-state-active]:-translate-y-[0.9rem] peer-data-[te-input-state-active]:scale-[0.8] motion-reduce:transition-none dark:text-neutral-200 dark:peer-focus:text-neutral-200"
								>{data.title}
							</label>
						</div>
					{/each}
				</div>
			</div>
		</div>
	</div>
	<div
		class="hidden opacity-0 opacity-100 transition-opacity duration-150 ease-linear data-[te-tab-active]:block"
		id="pills-profile"
		role="tabpanel"
		aria-labelledby="pills-profile-tab"
	>
		<div class="my-4 mx-8">
			<p class="mb-4">
				Do you have a quality product that needs an audience? We at DMart believe in joining hands
				with the right partners in order to provide high-quality yet affordable products to our
				customers. We invite suppliers to join us in our endeavour to offer the best to our
				customers. Be a part of our esteemed list of suppliers - with whom we have successful
				long-term partnerships - for a commercially satisfying and profitable relationship.
			</p>
			<p class="text-red-600 font-bold mb-4">
				We are temporarily suspending our "Tuesday Walk-ins" for all Vendors.
			</p>
			<p class="mb-4">
				You may continue to fill in the below form along with your product details. Our team will
				get in touch with you based on requirements.
			</p>
			<p class="mb-4">Fields marked with * are mandatory.</p>
			<div class="flex justify-between">
				<div class="w-1/2 p-4">
					<div class="font-bold underline underline-offset-4 my-4">Contact Details</div>
					{#each Data.partner as data}
						<div class="relative mb-3 xl:w-96 w-full" data-te-input-wrapper-init>
							<input
								type="text"
								class="peer block min-h-[auto] w-full rounded border-2 border-blue-400 bg-transparent py-[0.32rem] px-3 leading-[1.6] outline-solid transition-all duration-200 ease-linear focus:placeholder:opacity-100 data-[te-input-state-active]:placeholder:opacity-100 motion-reduce:transition-none dark:text-neutral-200 dark:placeholder:text-neutral-200 [&:not([data-te-input-placeholder-active])]:placeholder:opacity-0"
								id="exampleFormControlInput1"
								placeholder={data.placeholder}
							/>
							<label
								for="exampleFormControlInput1"
								class="pointer-events-none absolute top-0 left-3 mb-0 max-w-[90%] origin-[0_0] truncate pt-[0.37rem] leading-[1.6] text-neutral-500 transition-all duration-200 ease-out peer-focus:-translate-y-[0.9rem] peer-focus:scale-[0.8] peer-focus:text-primary peer-data-[te-input-state-active]:-translate-y-[0.9rem] peer-data-[te-input-state-active]:scale-[0.8] motion-reduce:transition-none dark:text-neutral-200 dark:peer-focus:text-neutral-200"
								>{data.title}
							</label>
						</div>
					{/each}
				</div>
				<div class="w-1/2 p-4">
					<div class="font-bold underline underline-offset-4 my-4">Product Details</div>
					{#each Data.product as data}
						<div class="relative mb-3 xl:w-96 w-full" data-te-input-wrapper-init>
							<input
								type="text"
								class="peer block min-h-[auto] w-full rounded border-2 border-blue-400 bg-transparent py-[0.32rem] px-3 leading-[1.6] outline-solid transition-all duration-200 ease-linear focus:placeholder:opacity-100 data-[te-input-state-active]:placeholder:opacity-100 motion-reduce:transition-none dark:text-neutral-200 dark:placeholder:text-neutral-200 [&:not([data-te-input-placeholder-active])]:placeholder:opacity-0"
								id="exampleFormControlInput1"
								placeholder={data.placeholder}
							/>
							<label
								for="exampleFormControlInput1"
								class="pointer-events-none absolute top-0 left-3 mb-0 max-w-[90%] origin-[0_0] truncate pt-[0.37rem] leading-[1.6] text-neutral-500 transition-all duration-200 ease-out peer-focus:-translate-y-[0.9rem] peer-focus:scale-[0.8] peer-focus:text-primary peer-data-[te-input-state-active]:-translate-y-[0.9rem] peer-data-[te-input-state-active]:scale-[0.8] motion-reduce:transition-none dark:text-neutral-200 dark:peer-focus:text-neutral-200"
								>{data.title}
							</label>
						</div>
					{/each}
				</div>
			</div>
		</div>
	</div>
</div>
