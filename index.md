---
#
# By default, content added below the "---" mark will appear in the home page
# between the top bar and the list of recent posts.
# To change the home page layout, edit the _layouts/home.html file.
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
# <h3 class="blackpar_title">(Models, Training and Inference)</h3>
layout: home
---
<div style="font-family: 'Source Sans Pro', sans-serif; background: url('/images/banner_no_text.png') no-repeat; background-size: cover; user-select: none;">
	<center>
		<h2 class="blackpar_title" >The 2<sup>nd</sup> workshop on<br>Efficient Natural Language and Speech Processing (ENLSP)</h2>
		<h3 class="blackpar_title">Friday Dec. 2nd 2022, New Orleans <br> <b>In-person</b> (Ballroom C) and <b>Virtual</b> </h3>
	</center>
</div>
<br>
<p>
The second version of the Efficient Natural Language and Speech Processing (ENLSP-II) workshop focuses on fundamental and challenging problems to make natural language and speech processing (especially pre-trained models) more efficient in terms of <b>Data, Model, Training, and Inference</b>. The workshop program offers an interactive platform for gathering different experts and talents from academia and industry through invited talks, panel discussion, paper submissions, reviews, interactive posters, oral presentations and a mentorship program. This will be a unique opportunity to address the efficiency issues of current models, build connections, exchange ideas and brainstorm solutions, and foster future collaborations. The topics of this workshop can be of interest for people working on general machine learning, deep learning, optimization, theory and NLP & Speech applications.
</p>

<br>

<!--
<div class="alert alert-danger" role="alert">
  <h4>Mentoring sessions announcement</h4>
  <p>
  The deadline for submitting papers to our second version of the Efficient Natural Language and Speech Processing (ENLSP-II) workshop is 25th of September. For that we will be scheduling two mentioring online sessions to answer your questions. Please join us:
  <br>
  <ul>
	<li>Tuesday the 6th of September 2022 from 10PM to 11PM (UTC-04:00)</li>
	<li>Wednesday the 7th of September 2022 from 9AM to 10AM (UTC-04:00)</li>
	<li>Tuesday the 13th of September 2022 from 10PM to 11PM (UTC-04:00): <a href="https://welink.zhumu.com/j/134854021">link</a></li>
	<li>Wednesday the 14th of September 2022 from 9AM to 10AM (UTC-04:00): <a href="https://welink.zhumu.com/j/130263276">link</a></li>
  </ul>
  </p>
</div>

<br>
-->

<h2 class="blackpar_title" id="overview">Overview</h2>
<p>
Pre-training a general model using self-supervised learning on huge amount of data and then fine-tuning that model on a specific task has become a generic paradigm in solving many natural language and speech processing tasks. Since then, we have had different types of pre-trained models (e.g. encoder-only such as BERT, decoder-only such as GPT, encoder-decoder such as T5) in very diverse range of scales (from millions to
more than 500 billion parameters) for different tasks.
<br><br>
There has been a common practice in the literature to increase the number of parameters of these pre-trained models to improve their performance or their zero/few-shot abilities. Despite the great success of these pre-trained models, it is evident that most of them are largely over-parameterized and their efficiency is under question. Training or deploying these models on devices or even cloud services with limited memory and computational power can be very expensive and challenging. For example, Megatron-Turing with 530B parameters has shown state-of-the-art results in many NLP tasks, but at the cost of using 560 DGX A100 nodes (more than 4000 NVIDIA A100) for training and using more than 300B tokens data. Moreover, delivering such huge models as a service to different clients will require different copies of the model for different tasks. Even fine-tuning the entire large model over a small labeled dataset can lead to overfitting. Therefore, it is of vital importance to invest on future of pre-trained models by enhancing their efficiency in terms of data, modeling, training and inference from different perspectives highlighted in this workshop.
</p>
<br>
<!-- Call for Papers -->
<h2 class="blackpar_title" id="call_for_papers">Call for Papers</h2>
We would like to share some fundamental challenges on improving efficiency of pre- trained models and encourage the NeurIPS community to submit their solutions, ideas, and ongoing work concerning data, model, training, and inference efficiency for NLP and speech processing. The scope of this workshop includes, but not limited to, the following topics:

<b>Efficient Pre-Training</b> Pre-training is a very expensive process. Even a small modification to the configuration of the models requires the user to redo pre-training.
<br>
<ul>
	<li>Accelerating the pre-training process</li>
	<li>Continual/Life-long pre-training and adapting pre-trained models to a new domain</li>
	<li>Efficient initialization and hyper-parameter tuning (HPT)</li>
	<li>Better pre-training self-supervised objectives</li>
	<li>Multi-domain pre-training</li>
	<li>Data vs. Scale of pre-trained models</li>
	<li>Pre-training Multimodal (e.g., text–speech) models</li>
	<li>New efficient architectures for pre-trained models</li>
</ul>


<b>Efficient Fine-tuning</b> Fine-tuning large pre-trained models on downstream tasks can be challenging because pre-trained models are very over-parameterized.
<br>
<ul>
	<li>Parameter-efficient tuning solutions to tune only a portion of the entire network (e.g. adapters)</li>
	<li>Efficient prompt-based fine-tuning</li>
	<li>Accelerating the fine-tuning process (e.g. optimizer, and layer-skipping)</li>
	<li>Efficient federated learning for NLP: reduce the communication costs, tackling heterogeneous data, heterogeneous models.</li>
</ul>


<b>Data Efficiency</b> Pre-trained models rely on a huge amount of unlabeled data which makes the training very sample inefficient.
<br>
<ul>
	<li>Sample efficient training, training with less data, few-shot and zero-shot learning</li>
	<li>Sample efficient data-augmentation, identifying which training samples should be augmented</li>
	<li>Data compression, data distillation</li>
	<li>Data selection, how to improve the quality of pre-training data</li>
</ul>

<b>Inference Efficiency</b> How can we reduce the inference time or memory footprint of a trained model for a particular task?
<br>
<ul>
	<li>Neural model compression techniques such as quantization, pruning, layer decomposition and knowledge distillation (KD) for NLP and Speech</li>
	<li>Impact of different compression techniques on the inductive biases learned by the original models</li>
	<li>Combined compression techniques for more efficient NLP and speech models</li>
	<li>Improving efficiency of KD by removing the teacher</li>
	<li>Extreme model compression (high compression ratio) for very large pre-trained language models</li>
</ul>

<b>Special Track) Efficient Graph Learning for NLP</b>
<br>
<ul>
	<li>Automatically transforming natural language into graph-structured data</li>
	<li>Representation learning on multi-relational or heterogeneous graphs</li>
	<li>Learning the mapping between complex data structures, like Graph2Seq, Graph2Tree, Graph2Graph</li>
	<li>Graph learning with pre-trained language models</li>
</ul>

<b>Other Efficient Applications</b> Pre-trained models are used in many tasks in NLP that efficiency can be their concern.
<br>
<ul>
	<li>Efficient Dense Retrieval</li>
	<li>Large language model as a service</li>
	<li>Training models on device</li>
	<li>Incorporating external knowledge into pre-trained models</li>
	<li>Unifying different pre-training models</li>
</ul>

<br>

<h2 class="blackpar_title">Submission Instructions</h2>
<p>
You are invited to submit your papers in our CMT submission <a href="https://cmt3.research.microsoft.com/ENLSP2022">portal</a>. All the submitted papers have to be anonymous for double-blind review. We expect each paper will be reviewed by at least three reviewers. The content of the paper (excluding the references and supplementary materials) should not be longer than 4 pages, strictly following the NeurIPS template style (which can be found <a href="https://neurips.cc/Conferences/2022/PaperInformation/StyleFiles">here</a>). 
<br /><br />
Authors can submit up to 100 MB of supplementary materials separately. Authors are highly encouraged to submit their codes for reproducibility purposes. According to the guideline of the NeurIPS workshops, already published papers are not encouraged for submission, but you are allowed to submit your ArXiv papers or the ones which are under submission. Moreover, a work that is presented at the main NeurIPS conference should not appear in a workshop. Please make sure to indicate the complete list of conflict of interests for all the authors of your paper. To encourage higher quality submissions, our sponsors are offering the <b>Best Paper</b> and the <b>Best Poster</b> Award to qualified outstanding original oral and poster presentations (upon nomination of the reviewers). Also, we will give one <b>outstading paper certification</b> for our special track of efficient graph learning for NLP.Bear in mind that our workshop is not archival, but the accepted papers will be hosted on the workshop website.
 

</p>

<br>

<h2 class="blackpar_title">Important Dates:</h2>
<p>
<ul>
	<li>Submission Deadline: <strike> September 25, 2022 AOE </strike> </li>
	<li>Acceptance Notification: <strike> October 20, 2022 AOE </strike> </li>
	<li>Camera-Ready Submission: <strike> November 1, 2022 AOE </strike> </li>
	<li>Workshop Date: <b>Friday December 2, 2022</b> (in-person and virtual)</li>
</ul>
</p>

<!--Confirmed Speakers-->
<h2 class="blackpar_title" id="speakers">Confirmed Speakers</h2>
<p>
{% include speakers.html %}
</p>


<h2 class="blackpar_title" id="speakers">Industrial Panelists</h2>
<p>
{% include panelists.html %}
</p>

<!-- Schedule -->
<h2 class="blackpar_title" id="schedule">Schedule (New Orleans Time Zone)</h2>
<p>
{% include schedule.html %}
</p>

<!-- Organizers -->
<h2 class="blackpar_title" id="organizers">Organizers</h2>
<p>
{% include organizers.html %}
</p>

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
	  <img src="/images/Soheila.png" alt="Soheila Samiee" class="img_card_perso">
	  <div class="container_perso">
		<center>
		<h6>
			<b>Soheila Samiee</b>
			<br>
			BASF
		</h6>
		</center>
	  </div>
	</div>
</div>


<br><br>

<!-- Technical Committee -->
<h2 class="blackpar_title" id="technical_committee">Technical Committee</h2>
<p>
{% include technical_committee.html %}
</p>
<br><br>

<h2 class="blackpar_title">Platinium Sponsor</h2>
<div class="row">
	<div class="col">
		<center>
			<img src="/images/huawei_logo.png">
		</center>
	</div>
	<div class="col">
		<center>
			<img src="/images/noahs_ark_lab_logo.png" width="250px">
		</center>
	</div>
</div>

<h2 class="blackpar_title">Gold Sponsor</h2>
<div class="row">
	<div class="col">
		<center>
			<img src="/images/BASF_logo.png" width="250px">
		</center>
	</div>
	<div class="col">
		<center>
			<img src="/images/rbc_logo.svg" width="250px">
		</center>
	</div>
</div>
