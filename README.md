# Hugging-Face-Summarizer

<div class="md:mt-2 lg:pr-20 xl:pr-24 2xl:pr-36"><div class="prose dark:prose-light"><h1 class="relative group flex items-center">
	<a rel="noopener nofollow" href="#bart-large-sized-model-fine-tuned-on-cnn-daily-mail" class="block pr-1.5 text-lg with-hover:absolute with-hover:p-1.5 with-hover:opacity-0 with-hover:group-hover:opacity-100 with-hover:right-full" id="bart-large-sized-model-fine-tuned-on-cnn-daily-mail">
		<span class="header-link"><svg viewBox="0 0 256 256" preserveAspectRatio="xMidYMid meet" height="1em" width="1em" role="img" aria-hidden="true" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns="http://www.w3.org/2000/svg" class="text-gray-500 hover:text-black w-4"><path fill="currentColor" d="M167.594 88.393a8.001 8.001 0 0 1 0 11.314l-67.882 67.882a8 8 0 1 1-11.314-11.315l67.882-67.881a8.003 8.003 0 0 1 11.314 0zm-28.287 84.86l-28.284 28.284a40 40 0 0 1-56.567-56.567l28.284-28.284a8 8 0 0 0-11.315-11.315l-28.284 28.284a56 56 0 0 0 79.196 79.197l28.285-28.285a8 8 0 1 0-11.315-11.314zM212.852 43.14a56.002 56.002 0 0 0-79.196 0l-28.284 28.284a8 8 0 1 0 11.314 11.314l28.284-28.284a40 40 0 0 1 56.568 56.567l-28.285 28.285a8 8 0 0 0 11.315 11.314l28.284-28.284a56.065 56.065 0 0 0 0-79.196z"></path></svg></span>
	</a>
	<span>
		BART (large-sized model), fine-tuned on CNN Daily Mail
	</span>
</h1>
<p>BART model pre-trained on English language, and fine-tuned on <a rel="noopener nofollow" href="https://huggingface.co/datasets/cnn_dailymail">CNN Daily Mail</a>. It was introduced in the paper <a rel="noopener nofollow" href="https://arxiv.org/abs/1910.13461">BART: Denoising Sequence-to-Sequence Pre-training for Natural Language Generation, Translation, and Comprehension</a> by Lewis et al. and first released in [this repository (<a rel="noopener nofollow" href="https://github.com/pytorch/fairseq/tree/master/examples/bart">https://github.com/pytorch/fairseq/tree/master/examples/bart</a>). </p>
<p>Disclaimer: The team releasing BART did not write a model card for this model so this model card has been written by the Hugging Face team.</p>
<h2 class="relative group flex items-center">
	<a rel="noopener nofollow" href="#model-description" class="block pr-1.5 text-lg with-hover:absolute with-hover:p-1.5 with-hover:opacity-0 with-hover:group-hover:opacity-100 with-hover:right-full" id="model-description">
		<span class="header-link"><svg viewBox="0 0 256 256" preserveAspectRatio="xMidYMid meet" height="1em" width="1em" role="img" aria-hidden="true" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns="http://www.w3.org/2000/svg" class="text-gray-500 hover:text-black w-4"><path fill="currentColor" d="M167.594 88.393a8.001 8.001 0 0 1 0 11.314l-67.882 67.882a8 8 0 1 1-11.314-11.315l67.882-67.881a8.003 8.003 0 0 1 11.314 0zm-28.287 84.86l-28.284 28.284a40 40 0 0 1-56.567-56.567l28.284-28.284a8 8 0 0 0-11.315-11.315l-28.284 28.284a56 56 0 0 0 79.196 79.197l28.285-28.285a8 8 0 1 0-11.315-11.314zM212.852 43.14a56.002 56.002 0 0 0-79.196 0l-28.284 28.284a8 8 0 1 0 11.314 11.314l28.284-28.284a40 40 0 0 1 56.568 56.567l-28.285 28.285a8 8 0 0 0 11.315 11.314l28.284-28.284a56.065 56.065 0 0 0 0-79.196z"></path></svg></span>
	</a>
	<span>
		Model description
	</span>
</h2>
<p>BART is a transformer encoder-encoder (seq2seq) model with a bidirectional (BERT-like) encoder and an autoregressive (GPT-like) decoder. BART is pre-trained by (1) corrupting text with an arbitrary noising function, and (2) learning a model to reconstruct the original text.</p>
<p>BART is particularly effective when fine-tuned for text generation (e.g. summarization, translation) but also works well for comprehension tasks (e.g. text classification, question answering). This particular checkpoint has been fine-tuned on CNN Daily Mail, a large collection of text-summary pairs.</p>
<h2 class="relative group flex items-center">
	<a rel="noopener nofollow" href="#intended-uses--limitations" class="block pr-1.5 text-lg with-hover:absolute with-hover:p-1.5 with-hover:opacity-0 with-hover:group-hover:opacity-100 with-hover:right-full" id="intended-uses--limitations">
		<span class="header-link"><svg viewBox="0 0 256 256" preserveAspectRatio="xMidYMid meet" height="1em" width="1em" role="img" aria-hidden="true" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns="http://www.w3.org/2000/svg" class="text-gray-500 hover:text-black w-4"><path fill="currentColor" d="M167.594 88.393a8.001 8.001 0 0 1 0 11.314l-67.882 67.882a8 8 0 1 1-11.314-11.315l67.882-67.881a8.003 8.003 0 0 1 11.314 0zm-28.287 84.86l-28.284 28.284a40 40 0 0 1-56.567-56.567l28.284-28.284a8 8 0 0 0-11.315-11.315l-28.284 28.284a56 56 0 0 0 79.196 79.197l28.285-28.285a8 8 0 1 0-11.315-11.314zM212.852 43.14a56.002 56.002 0 0 0-79.196 0l-28.284 28.284a8 8 0 1 0 11.314 11.314l28.284-28.284a40 40 0 0 1 56.568 56.567l-28.285 28.285a8 8 0 0 0 11.315 11.314l28.284-28.284a56.065 56.065 0 0 0 0-79.196z"></path></svg></span>
	</a>
	<span>
		Intended uses &amp; limitations
	</span>
</h2>
<p>You can use this model for text summarization. </p>
<h3 class="relative group flex items-center">
	<a rel="noopener nofollow" href="#how-to-use" class="block pr-1.5 text-lg with-hover:absolute with-hover:p-1.5 with-hover:opacity-0 with-hover:group-hover:opacity-100 with-hover:right-full" id="how-to-use">
		<span class="header-link"><svg viewBox="0 0 256 256" preserveAspectRatio="xMidYMid meet" height="1em" width="1em" role="img" aria-hidden="true" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns="http://www.w3.org/2000/svg" class="text-gray-500 hover:text-black w-4"><path fill="currentColor" d="M167.594 88.393a8.001 8.001 0 0 1 0 11.314l-67.882 67.882a8 8 0 1 1-11.314-11.315l67.882-67.881a8.003 8.003 0 0 1 11.314 0zm-28.287 84.86l-28.284 28.284a40 40 0 0 1-56.567-56.567l28.284-28.284a8 8 0 0 0-11.315-11.315l-28.284 28.284a56 56 0 0 0 79.196 79.197l28.285-28.285a8 8 0 1 0-11.315-11.314zM212.852 43.14a56.002 56.002 0 0 0-79.196 0l-28.284 28.284a8 8 0 1 0 11.314 11.314l28.284-28.284a40 40 0 0 1 56.568 56.567l-28.285 28.285a8 8 0 0 0 11.315 11.314l28.284-28.284a56.065 56.065 0 0 0 0-79.196z"></path></svg></span>
	</a>
	<span>
		How to use
	</span>
</h3>
<p>Here is how to use this model with the <a rel="noopener nofollow" href="https://huggingface.co/transformers/main_classes/pipelines.html">pipeline API</a>:</p>
<pre><code class="language-python"><span class="hljs-keyword">from</span> transformers <span class="hljs-keyword">import</span> pipeline

summarizer = pipeline(<span class="hljs-string">"summarization"</span>, model=<span class="hljs-string">"facebook/bart-large-cnn"</span>)

ARTICLE = <span class="hljs-string">""" New York (CNN)When Liana Barrientos was 23 years old, she got married in Westchester County, New York.</span>
<span class="hljs-string">A year later, she got married again in Westchester County, but to a different man and without divorcing her first husband.</span>
<span class="hljs-string">Only 18 days after that marriage, she got hitched yet again. Then, Barrientos declared "I do" five more times, sometimes only within two weeks of each other.</span>
<span class="hljs-string">In 2010, she married once more, this time in the Bronx. In an application for a marriage license, she stated it was her "first and only" marriage.</span>
<span class="hljs-string">Barrientos, now 39, is facing two criminal counts of "offering a false instrument for filing in the first degree," referring to her false statements on the</span>
<span class="hljs-string">2010 marriage license application, according to court documents.</span>
<span class="hljs-string">Prosecutors said the marriages were part of an immigration scam.</span>
<span class="hljs-string">On Friday, she pleaded not guilty at State Supreme Court in the Bronx, according to her attorney, Christopher Wright, who declined to comment further.</span>
<span class="hljs-string">After leaving court, Barrientos was arrested and charged with theft of service and criminal trespass for allegedly sneaking into the New York subway through an emergency exit, said Detective</span>
<span class="hljs-string">Annette Markowski, a police spokeswoman. In total, Barrientos has been married 10 times, with nine of her marriages occurring between 1999 and 2002.</span>
<span class="hljs-string">All occurred either in Westchester County, Long Island, New Jersey or the Bronx. She is believed to still be married to four men, and at one time, she was married to eight men at once, prosecutors say.</span>
<span class="hljs-string">Prosecutors said the immigration scam involved some of her husbands, who filed for permanent residence status shortly after the marriages.</span>
<span class="hljs-string">Any divorces happened only after such filings were approved. It was unclear whether any of the men will be prosecuted.</span>
<span class="hljs-string">The case was referred to the Bronx District Attorney\'s Office by Immigration and Customs Enforcement and the Department of Homeland Security\'s</span>
<span class="hljs-string">Investigation Division. Seven of the men are from so-called "red-flagged" countries, including Egypt, Turkey, Georgia, Pakistan and Mali.</span>
<span class="hljs-string">Her eighth husband, Rashid Rajput, was deported in 2006 to his native Pakistan after an investigation by the Joint Terrorism Task Force.</span>
<span class="hljs-string">If convicted, Barrientos faces up to four years in prison.  Her next court appearance is scheduled for May 18.</span>
<span class="hljs-string">"""</span>
print(summarizer(ARTICLE, max_length=<span class="hljs-number">130</span>, min_length=<span class="hljs-number">30</span>, do_sample=<span class="hljs-literal">False</span>))
<span class="hljs-meta">&gt;&gt;&gt; </span>[{<span class="hljs-string">'summary_text'</span>: <span class="hljs-string">'Liana Barrientos, 39, is charged with two counts of "offering a false instrument for filing in the first degree" In total, she has been married 10 times, with nine of her marriages occurring between 1999 and 2002. She is believed to still be married to four men.'</span>}]
</code></pre>
<h3 class="relative group flex items-center">
	<a rel="noopener nofollow" href="#bibtex-entry-and-citation-info" class="block pr-1.5 text-lg with-hover:absolute with-hover:p-1.5 with-hover:opacity-0 with-hover:group-hover:opacity-100 with-hover:right-full" id="bibtex-entry-and-citation-info">
		<span class="header-link"><svg viewBox="0 0 256 256" preserveAspectRatio="xMidYMid meet" height="1em" width="1em" role="img" aria-hidden="true" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns="http://www.w3.org/2000/svg" class="text-gray-500 hover:text-black w-4"><path fill="currentColor" d="M167.594 88.393a8.001 8.001 0 0 1 0 11.314l-67.882 67.882a8 8 0 1 1-11.314-11.315l67.882-67.881a8.003 8.003 0 0 1 11.314 0zm-28.287 84.86l-28.284 28.284a40 40 0 0 1-56.567-56.567l28.284-28.284a8 8 0 0 0-11.315-11.315l-28.284 28.284a56 56 0 0 0 79.196 79.197l28.285-28.285a8 8 0 1 0-11.315-11.314zM212.852 43.14a56.002 56.002 0 0 0-79.196 0l-28.284 28.284a8 8 0 1 0 11.314 11.314l28.284-28.284a40 40 0 0 1 56.568 56.567l-28.285 28.285a8 8 0 0 0 11.315 11.314l28.284-28.284a56.065 56.065 0 0 0 0-79.196z"></path></svg></span>
	</a>
	
# Step by Step implementation is done in above mentioned Notebook
