<!-- Navbar.vue -->
<template>

  <div>
  
    <div class="title-container">
      <h4 class="text-center title" >
        <img :src="paper" width="70" height="70" class="d-inline-block align-center" alt="">
        News Benchmark: Systematic Evaluation of LLMs for Writing Proficiency and Safety Adherence in Chinese Journalistic Editorial Applications
      </h4>
    </div>

    <br/>

    <div class="container">
      <p class="author text-center">
        <a href="#" style="white-space: nowrap">Miao Li</a><sup>1</sup> and 
        <a href="#" style="white-space: nowrap">Ming-Bin Chen</a><sup>1</sup> and 
        <a href="#" style="white-space: nowrap">Bo Tang</a><sup>2</sup> and 
        <a href="#" style="white-space: nowrap">Shengbin Hou</a><sup>3</sup> and 
        <a href="#" style="white-space: nowrap">Pengyu Wang</a><sup>3</sup> and 
        <a href="#" style="white-space: nowrap">Haiying Deng</a><sup>4</sup> and 
        <a href="#" style="white-space: nowrap">Zhiyu Li</a><sup>2</sup> and 
        <a href="#" style="white-space: nowrap">Feiyu Xiong</a><sup>2</sup> and 
        <a href="#" style="white-space: nowrap">Keming Mao</a><sup>3</sup> and 
        <a href="#" style="white-space: nowrap">Peng Cheng</a><sup>4</sup> and 
        <a href="#" style="white-space: nowrap">Yi Luo</a><sup>4</sup>
      </p>
    </div>

    <div class="container">
      <p class="author text-center">
        <a style="white-space: nowrap;font-size: medium;"><sup>1</sup>The University of Melbourne, Australia</a>&nbsp;&nbsp;&nbsp;
        <a style="white-space: nowrap;font-size: medium;"><sup>2</sup>IAAR, China</a>&nbsp;&nbsp;&nbsp;
        <a style="white-space: nowrap;font-size: medium;"><sup>3</sup>Northeastern University, China</a>&nbsp;&nbsp;&nbsp;
        <a style="white-space: nowrap;font-size: medium;"><sup>4</sup>State Key Laboratory of Media Convergence Production Technology and Systems, China</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
      </p>

      <p class="author text-center" style="font-size: medium; color: grey;">
        miao4@student.unimelb.edu.au, tangb@iaar.ac.cn
      </p>
    </div>


    <div class="container text-center">
      <button type="button" class="btn btn-dark"><a href="#" style="color: white;">Code</a></button>&nbsp;&nbsp;&nbsp;
      <button type="button" class="btn btn-dark"><a href="https://arxiv.org/abs/2403.00862" style="color: white;">Paper</a></button>
    </div>

    <br/>
    <br/>

    <div class="container text-center">
      <h2 class="title" style="text-align: center;">Abstract</h2>
      <p class="paragraph">This study presents NewsBench, a novel benchmak framework developed to evaluate the capabiity of Large Lanquage Models (lMs)in Chinese jouralisticWriting Proficiency (JWP) and their Safety Adherence (SA), addressing the gap between journalistic ethics and the risks associated with Al utilization. Comprising1.267 tasks across 5 editoral applications, 7 aspects (incuding safety and iouralisic wrting with 4 detaled facets), and spanning 24 news topics domains,NewsBench emplys wo GPT-4 based automalic evalualion proiocols validated by buman assessment Our comprehensive anawsis of 41 ulMs highightedGPT-4 and ERNlE Bot as top performers, yet revealed a relative deficiency in joumalisic ethic adherence duing creative wrting tasks. These findings underscorthe need for enhanced ethical quidance in Al-generated joumalisic content, marking a step fonward in aigning Al capablies with jouralistic standards andsafety considerations.</p>
    </div>
    

    <br/>


    <div class="jumbotron jumbotron-fluid text-center" style="background-color:aliceblue;">
      <div class="container">
        <h5 class="display-4">Overview</h5>
      </div>
    </div>

    <br/>

    <div class="p-container">
      <p class="paragraph">The widespread adoption of Large Language Models (LLMs) such as OpenAI's ChatGPT has prompted discussions on the responsible use of this technology due to its non-deterministic nature. While efforts have been made to address safety concerns, there is a lack of standardized benchmarks for evaluating LLMs' alignment with journalistic ethics. To bridge this gap, this paper introduces NewsBench, a comprehensive benchmark evaluation framework for assessing LLMs in journalistic writing and safety compliance. Through automatic evaluation protocols and comparative analysis of 11 LLMs, including GPT-4 and ERNIE Bot, this study identifies their strengths and weaknesses in adhering to journalistic standards. Our key contributions are:</p>
      <p class="paragraph" style="width: 90%;margin: 0 auto;">• Developed NewsBench, a benchmark for evaluating LLMs on journalistic writing and safety, featuring generative and multiplechoice tasks across 5 applications and 7 aspects.</p>
      <br/>
      <p class="paragraph" style="width: 90%;margin: 0 auto;">• Introduced two GPT-4-based evaluation protocols for journalistic writing proficiency and safety compliance, validated by human annotation</p>
      <br/>
      <p class="paragraph" style="width: 90%;margin: 0 auto;">• Conducted a comparative analysis and error assessment of 11 LLMs, identifying strengths and weaknesses.</p>
      <br/>
      <p class="paragraph" style="width: 90%;margin: 0 auto;">• Identified GPT-4 and ERNIE Bot as leading models, highlighting their limitations in adhering to journalistic ethics in creative writing tasks.</p>
    </div>

    <br/>

    <br/>


    <div class="jumbotron jumbotron-fluid text-center" style="background-color:aliceblue;">
      <div class="container">
        <h5 class="display-4">Framework</h5>
      </div>
    </div>

    <br/>

    <div class="p-container">
      <p class="paragraph">The benchmark evaluates two principal criteria: Journalistic Writing Proficiency (JWP) and Safety Adherence (SA) in content generated by LLMs. Our framework includes both open-ended generation tasks and multiple-choice tasks, with 4 subsets totaling 1267 tasks: JWP generation tasks, JWP multiple choice tasks, SA generation tasks, and SA multiple choice tasks. Each subset covers 5 common journalistic editorial applications and up to 24 domains.</p>
      <p class="paragraph">Figure 1 illustrates the comprehensive design of the NewsBench evaluation framework. Tasks from four subsets are inputted into a targeted LLM to elicit corresponding multiple-choice answers and generated textual responses. Two specialized automatic evaluation protocols based on GPT-4 assess the LLM's Journalistic Writing Proficiency and Safety Adherence.</p>
      <img :src="newsbench_architecture" style="width: 50%; height: 50%;" class="rounded mx-auto d-block" alt="...">
      <figcaption class="figure-caption">Figure 1: The key components and processes of the NewsBench benchmark. The numbers inside the brackets indicate the task counts for the subsets. The bold border boxes are the output scores</figcaption>
      <!-- <p class="paragraph">Fine-grained aspects for JWP and SA ensure a comprehensive evaluation of LLM-generated content against journalistic writing standards and safety adherence requirements. JWP is defined with four aspects: Language Fluency, Logical Coherence, Style Alignment, and Instruction Fulfillment. SA is examined across six aspects: Civil Language, Bias and Discrimination, Personal Privacy, Social Harm, Journalistic Ethics, and Illegal Activities.</p>
      <p class="paragraph">Tasks are assigned editorial application scenarios, focusing on the editorial phase to position LLMs as editorial assistants. Applications such as headline generation, summarization, continuation of writing, expansion of writing, and style refinement are covered.</p>
      <p class="paragraph">Each task features a prompt crafted according to a specific triplet setting, including task type, application, and target aspects. Instructions provide context and serve as input for LLMs. Some tasks emphasize safety performance through adversarial instructions.</p>
      <p class="paragraph">The dataset comprises 1267 tasks, distributed across two question types, five applications, seven aspects, and 24 domains. Each task underwent careful construction and review, with detailed instructions and human-written answers provided for potential extended use beyond the evaluation framework.</p> -->
    </div>

    <br/>
    <br/>

    <div class="jumbotron jumbotron-fluid text-center" style="background-color:aliceblue;">
      <div class="container">
        <h5 class="display-4">Evalutation Protocol</h5>
      </div>
    </div>

    <br/>

    <div class="p-container">
      <p class="paragraph">Our evaluation framework automates the assessment of large language models in journalistic writing proficiency and safety adherence, utilizing two automatic evaluation protocols based on recent advancements in natural language generation evaluation methodologies. We comprehensively evaluate journalistic writing proficiency, considering language fluency, logical coherence, style alignment, and instruction fulfillment, while providing tailored evaluation prompts for each safety aspect to ensure validity and reliability.Table 1 shows the evaluation prompts for the 6 SA aspects.</p>
      <img :src="prompt" style="width: 70%; height: 70%;" class="rounded mx-auto d-block" alt="...">
      <figcaption class="figure-caption" >Table 1: Evaluation prompts for the 6 SA aspects</figcaption>
      <p class="paragraph"></p>
      <p class="paragraph"></p>
      <p class="paragraph"></p>
    </div>

    <br/>
    <br/>

    <div class="jumbotron jumbotron-fluid text-center" style="background-color:aliceblue;">
      <div class="container">
        <h5 class="display-4">Main Results</h5>
      </div>
    </div>

    <br/>

    <div class="p-container">
      <p class="paragraph">We evaluated 11 LLMs capable of generating Chinese text, including GPT-4-1106, GPT-3.5-turbo, ERNIE Bot, Baichuan2-13B, Baichuan2-53B, ChatGLM2-6B, ChatGLM3-6B, Aquila-34B, InternLM-20B, Qwen-14B, Xinyu2-70B, and Xverse. These models cover corpora ranging from 2.6 trillion to 3.2 trillion tokens. Our evaluation spanned 1,267 benchmark samples.</p>
      <img :src="score" style="width: 80%; height: 80%;" class="rounded mx-auto d-block" alt="...">
      <figcaption class="figure-caption" >Table 2: Evaluated large language models capable of generating Chinese.</figcaption>
      <p class="paragraph">In Table 2,in tasks related to journalistic writing proficiency, GPT-4-1106 emerged as the top performer, while ERNIE Bot showcased notable performance in safety evaluation and multiple-choice questions. Further analysis revealed that model size is not the sole determinant of performance; model architecture and training methodologies are equally crucial. ERNIE Bot demonstrated outstanding performance in addressing bias and discrimination, particularly excelling in summarization tasks. These findings shed light on the nuanced strengths of different models in the realm of journalistic writing proficiency.</p>
    </div>

    <br/>
    <br/>

    <div class="jumbotron jumbotron-fluid text-center" style="background-color:aliceblue;">
      <div class="container">
        <h5 class="display-4">Limitations</h5>
      </div>
    </div>

    <br/>

    <div class="p-container" style="display: flex;">
      <div style="width: 50%;">
        <h4 style="text-align: left;">Limitations</h4>
        <p style="font-size: medium;">There are several limitations to this study. Firstly, our dataset is exclusively in Chinese, limiting the applicability of the evaluation framework to other languages. Secondly, while our benchmark dataset is substantial, plans for expansion are in place to enhance comprehensiveness. The uneven distribution of samples across contexts is noted as well. Thirdly, the framework relies solely on the implicit knowledge embedded within LLMs for evaluation, which may result in inaccuracies when external evidence is required.</p>
      </div>
      <div style="width: 10%;"><p> </p></div>
      <div style="width: 50%;">
        <h4 style="text-align: left;">Constraints</h4>
        <p style="font-size: medium;">The dataset is limited to Chinese, potentially limiting its applicability to other languages. Uneven sample distribution and sole reliance on LLMs' embedded knowledge, lacking external evidence, may lead to inaccuracies. The exclusion of certain essential editorial applications reflects a limitation in comprehensively assessing journalistic integrity within the framework.
          Besides,please note that this content contains examples of impolite or sensitive language related to news safety issues. Sensitive individuals may wish to disregard.</p>
      </div>
    </div>

    <br/><br/>

    <div class="p-container">
      <h3 style="text-align: left;">BibTeX</h3>
      <pre style="background-color: lightgrey;"><code style="font-size: small;">
  @misc{li2024newsbench,
        title={NewsBench: Systematic Evaluation of LLMs for Writing Proficiency and Safety Adherence in Chinese Journalistic Editorial Applications}, 
        author={Miao Li and Ming-Bin Chen and Bo Tang and Shengbin Hou and Pengyu Wang and Haiying Deng and Zhiyu Li and Feiyu Xiong and Keming Mao and Peng Cheng and Yi Luo},
        year={2024},
        eprint={2403.00862},
        archivePrefix={arXiv},
        primaryClass={cs.CL}
  }
      </code></pre>
    </div>
    
  </div>

</template>

<script>
export default {
  name: 'MyHome',
  data(){
    return {
      paper: require('../assets/paper.png'),
      newsbench_architecture: require('../assets/newsbench_architecture1.png'),
      prompt: require('../assets/prompt.png'),
      score: require('../assets/score.png'),
    }
  }
}
</script>

<style>
  h4 {
    text-align: center;
    margin-top: 50px;
    font-weight: bold;
  }

  .paragraph {
    text-align: justify;
    margin-top: 30px; /* 与h3保持一段距离 */
    font-size: medium;
  }

  footer {
    text-align: center;
    margin-top: 100px;
  }

  .p-container {
  width: 55%; /* 表格容器占据页面宽度的70% */
  margin: 0 auto; /* 居中显示 */
  }
  .title-container {
    width: 70%; /* 表格容器占据页面宽度的70% */
    margin: 0 auto; /* 居中显示 */
    font-weight: bold;
  }

  a{
    text-decoration: none;
  }
  .container{
    width: 50%; /* 表格容器占据页面宽度的70% */
    margin: 0 auto; /* 居中显示 */
  }
  .figure-caption {
    text-align: center; width: 90%;
    font-size: small;
  }

</style>