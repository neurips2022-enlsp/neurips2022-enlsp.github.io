---
#
# By default, content added below the "---" mark will appear in the home page
# between the top bar and the list of recent posts.
# To change the home page layout, edit the _layouts/home.html file.
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
layout: home
---
<div id="banner">
	<center>
	<h2 class="blackpar_title">The 2<sup>nd</sup> workshop on<br>Efficient Natural Language and Speech Processing (ENLSP)</h2>
	<h3 class="blackpar_title">(Models, Training and Inference)</h3>
	</center>
</div>

<p>
TBD description

<br><br>

<h2 class="blackpar_title" id="overview">Overview</h2>
<p>
TBD
</p>

<!-- Call for Papers -->
<h2 class="blackpar_title" id="call_for_papers">Call for Papers</h2>
We encourage the NeurIPS community to submit their solutions, ideas, and ongoing work concerning data, model, training, and inference efficiency for NLP and speech processing. The scope of this workshop includes, but not limited to, the following topics.

<br /><br />
<b>Efficient Pre-Training and Fine-Tuning.</b> Pre-training is a very expensive process. Even a small modification to the configuration of the models requires the user to redo pre-training:
<br />

<ul>
	<li>Fast pre-training techniques, avoiding pre-training from scratch</li>
	<li>Multi-domain pre-training/fine-tuning and fast domain adaptation for pre-trained/fine tuned models</li>
	<li>Multimodal pre-trained (e.g., text--speech) models</li>
	<li>Avoiding task-specific fine tuning of pre-trained models</li>
	<li>New efficient architectures for pre-trained models</li>
</ul>

<br />
<b>Model Compression.</b> Neural model compression techniques such as quantization, pruning, layer decomposition and knowledge distillation (KD) aim at reducing the number of parameters of the models, improving their memory requirements or running efficiency:
<br />

<ul>
	<li>Impact of different compression techniques on the inductive biases learned by the original models</li>
	<li>Combined compression techniques for more efficient NLP and speech models</li>
	<li>Efficient KD for NLP and speech, efficient intermediate layer distillation, and teacher-free distillation</li>
	<li>Improving KD for large classification problems (e.g., text generation and machine translation with a very large number of output classes)</li>
	<li>Solving the <i>Capacity Gap</i> problem and the <i>Search Problem</i> associated with finding the best checkpoint of the teacher</li>
	<li>Theory of KD (e.g., how does KD work?) </li>
</ul>

<br />
<b>Efficient Training.</b> How to improve the training speed of the NLP and speech models:
<br />
<ul>
	<li>Improving the optimizer for faster training</li>
	<li>Accelerated training of different tasks in NLP and speech</li>
	<li>Distributed training,  federated learning and continual learning for NLP and speech tasks </li>
</ul>

<br />
<b>Data Efficiency.</b> Pre-trained models rely on a huge amount of unlabeled data which makes the training very sample inefficient:
<br />
<ul>
	<li>Sample efficient training, training with less data, few-shot and zero-shot learning</li>
	<li>Sample efficient data-augmentation, identifying which training samples should be augmented</li>
	<li>Low-resource NLP and speech, considering training tasks with limited available data</li>
</ul>

<br />
<b>Edge Intelligence.</b>  Running the trained models on edge devices will require a conversion process to match the network with hardware specifications:
<br />
<ul>
	<li>TinyML for NLP and speech on embedded systems</li>
	<li>Efficient conversion versus hardware-aware training</li>
	<li>Training on device</li>
</ul>

<h2 class="blackpar_title">Submission Instructions</h2>
<p>
TBD
</p>

<h2 class="blackpar_title">Important Dates:</h2>
<p>
TBD
</p>

<!--Confirmed Speakers-->
<h2 class="blackpar_title" id="speakers">Confirmed Speakers</h2>
{% include speakers.html %}

<h2 class="blackpar_title" id="speakers">Panelists</h2>
{% include panelists.html %}

<!-- Schedule -->
<h2 class="blackpar_title" id="schedule">Schedule (EST time zone - New York/Montreal/Toronto)</h2>
{% include schedule.html %}

<!-- Organizers -->
<h2 class="blackpar_title" id="organizers">Organizers</h2>
{% include organizers.html %}

<h2 class="blackpar_title" id="Organizers">Volunteers</h2>
<div class="row_perso">
	<div class="card_perso column_perso justify-content-center" style="margin-left:24%;">
	  <img src="/images/khalil_bibi.png" alt="Khalil Bibi" class="img_card_perso">
	  <div class="container_perso" >
		<center>
		<h6>
			<b>Khalil Bibi</b>
			<br>
			Huawei Noah's Ark Lab
		</h6>
		</center>
	  </div>
	</div>
	<div class="card_perso column_perso">
	  <img src="/images/anderson_avilla.jpg" alt="Anderson Avilla" class="img_card_perso">
	  <div class="container_perso">
		<center>
		<h6>
			<b>Andrson Avilla</b>
			<br>
			Huawei Noah's Ark Lab
		</h6>
		</center>
	  </div>
	</div>
</div>


<br><br>

<!-- Technical Committee -->
<h2 class="blackpar_title" id="technical_committee">Technical Committee</h2>
{% include technical_committee.html %}
<br><br>

<h2 class="blackpar_title">Sponsor</h2>
<center>
	<img src="/images/logos.png">	
</center>