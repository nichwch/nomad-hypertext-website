<script lang="ts">
</script>

<svelte:head>
	<title>Nomad Hypertext</title>
	<meta name="description" content="A writing app built around semantic search" />
</svelte:head>

<div class="pt-10 h-full">
	<div class="w-full px-10 lg:w-[30rem] lg:mx-auto">
		<img
			class="block w-52 mx-auto"
			alt="nomad hypertext logo, a horse"
			src="nomadhypertextlogo.png"
		/>
		<h1 class="text-3xl mb-1 text-center">NOMAD HYPERTEXT</h1>
		<h3 class="text-xl mb-3 text-center">A local-first writing app built around semantic search</h3>
		<h3 class=" text-center">
			Made by <a href="https://nicholaschen.io"> Nicholas Chen</a> at the
			<a href="https://recurse.com">Recurse Center</a>
		</h3>
		<h3 class=" italic text-center">
			<a href="https://github.com/nichwch/nomad-hypertext/releases">Available on MacOS</a>
		</h3>
	</div>

	<video
		autoplay
		muted
		loop
		class="  w-full border-y border-y-black lg:border-x lg:border-x-black lg:w-[50rem] lg:mx-auto my-10 p-0 px-0"
		src="nomadhypertextdemo.mp4"
	>
		<track kind="captions" />
	</video>
	<div class="w-full px-10 lg:w-[30rem] lg:mx-auto">
		<p
			class="first-letter:float-left first-letter:text-5xl first-letter:mr-1 first-letter:text-red-800"
		>
			N<span class="small-caps text-red-800">omad Hypertext </span> is a writing app built around
			semantic search. It lets you see connections between your ideas in real time as your write -
			click on the
			<span class="text-red-800">#</span> symbol next to a paragraph, and similar ideas you've written
			about in the past will show in the sidebar. This helps you spot both recurring themes and unexpected
			links between seemingly different ideas.
		</p>
		<p>
			Nomad Hypertext works completely offline and is free and <a
				href="https://github.com/nichwch/nomad-hypertext">open source.</a
			>
		</p>
		<h2>Effort-free organization</h2>
		<p class="mt-5 italic">
			"I do not want to hamper myself with anything in preparing my notes. I will not introduce any
			order or system. Whatever I recall, I will write down"
		</p>
		<p>- Dostoevsky, Notes From Underground</p>
		<p class=" mt-5">
			Unlike other writing apps, there is no need to manually tag ideas or manually draw links
			between documents. Semantic search itself is the primary method of organization, and it works
			automatically in the background, leaving you free to write down your ideas freely. This makes
			it an ideal tool for journaling, brainstorming, and ideation.
		</p>
		<p>
			You can think of it as Nomad Hypertext "semantically hyperlinking" ideas together in the
			background automatically as your write.
		</p>
		<p class="italic">
			<a href="https://blog.nicholaschen.io/posts/What%20is%20Nomad%20Hypertext.txt"
				>[Read more about Nomad Hypertext]</a
			>
		</p>
		<h2>Totally offline</h2>
		<p class=" mt-5">
			Nomad Hypertext embeds what you write into a local vector database using a local AI model in
			real time. All of this happens on your device, completely offline. You can use Nomad Hypertext
			on a plane, in a forest, on the Eurasian steppe - anywhere life takes you.
		</p>
		<h2>Plaintext!</h2>
		<p>
			Because Nomad Hypertext does not rely on tags or backlinks to organize ideas, it does not need
			any proprietary data format - your notes are plain text files. This means you can easily take
			your notes to another app (Obsidian perhaps), back them up using Git, pipe them into LLM
			command line tools, or feed them into a static site generator.
		</p>
		<p>Plain text is simple, portable, and compatible with everything - truly nomadic.</p>
		<h2>Yurt</h2>
		<p>
			Speaking of static site generators, Nomad Hypertext has a sister project: <a
				href="https://github.com/nichwch/yurt">Yurt</a
			>, a static site generator that semantically hyperlinks paragraphs for you automatically.
		</p>
		<p>
			At build time, it embeds all your posts into vectors and puts them into a vector database.
			Then, for each paragraph in a post, it queries the vector database for the 20 most similar
			paragraphs from all your notes. It stores these in a precomputed index. It then statically
			generates a blog for you (like Gatsby or any other static site generator), and uses this index
			so users can see related ideas when they click on a paragraph.
		</p>
		<p>
			You can learn more about Yurt on my blog <a
				href="https://blog.nicholaschen.io/posts/What%20is%20Yurt.txt">here</a
			> - which is itself deployed using Yurt.
		</p>
		<p>
			You can deploy your own semantically hyperlinked blog using Yurt! <a
				href="https://github.com/nichwch/yurt">The repo is a template repo</a
			>
			- clone it and follow the instructions in the README to get started.
		</p>
		<h2>Get Nomad Hypertext</h2>
		<p>Nomad Hypertext is available on MacOS now.</p>
		<p class="italic mt-5">
			<a href="https://github.com/nichwch/nomad-hypertext/releases">[DOWNLOAD NOMAD HYPERTEXT]</a>
		</p>
	</div>
	<img
		class="block py-32 w-full px-5 lg:w-[36rem] lg:mx-auto"
		alt="robot riding a horse"
		src="nomadhypertext.png"
	/>
</div>

<style>
	p {
		margin-top: 1.25rem;
	}
	a {
		color: blue;
		text-decoration: underline;
	}
	h2 {
		margin-top: 2.5rem;
		font-size: 1.5rem /* 24px */;
		line-height: 2rem /* 32px */;
	}
	a:visited {
		color: purple;
	}
</style>
