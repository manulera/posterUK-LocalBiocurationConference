
<div class="box full">

# 😥 The problem 😥

<div class="content">

We can describe sequence features in open formats (such as `.gb`), but not cloning strategies.

Let's imagine a typical strategy to clone a gene into a plasmid:

<div class="img-wrapper">
    <img width="90%" src="cloning_strategy.svg" alt="">
</div>

1. Amplify the DNA from the organism using PCR with oligonucleotides that contain 5' extensions.
2. Digest the plasmid and PCR product with digestion enzymes.
3. Ligate the digested products.

<!-- 🤔 Well, there must be an Open Standard to encode this since this is routinely done in **hundreds of laboratories**.

<div class="alert alert-danger text-center mx-auto" role="alert" style="width:fit-content"><strong>🚨Spoiler alert🚨</strong><br>That is not the case</div> -->

<div class="img-wrapper">
    <img width="60%" src="meme.svg" alt="">
</div>

</div>
</div>

<div class="box full">

# 🤔 The solution? 🤔

<div class="content">

In ShareYourCloning, we use `json` to document two types of sequence sources:

## 1. Sequence is newly generated

<div class="mermaid">
graph LR;
    A[<code>Sequence<hr>id: 1</code>]-->C["<code>Source<hr>id: 3<br>input: [1,2]<br>output: 4<br>experiment_specific_stuff<br>...</code>"];
    B[<code>Sequence<hr>id: 2</code>]-->C;
    C-->D[<code>Sequence<hr>id: 4</code>];
</div>

## 2. Sequence in collection / naturally occurring

<div class="mermaid">
graph LR;
    B["<code>Source<hr>id: 1<br>input: []<br>output: 2<br>request_to_your<br>favourite_database</code>"]-->A[<code>Sequence<hr>id: 2</code>];
    C["<code>Source<hr>id: 1<br>input: []<br>output: 2<br>a_file</code>"]-->D[<code>Sequence<hr>id: 2</code>];
</div>

Enter 🔥🔥 **ShareYourCloning** 🔥🔥, a web application where you can simulate your cloning strategy and export it in this format to share with others or for publication.</div>

<div class="img-wrapper">
    <img width="80%" src="architecture2.svg" alt="">
</div>



</div>
</div>

<div class="box full">

# 🙋 Try it yourself! 🙋‍♂️

<div class="content centered">

<a href="https://shareyourcloning.netlify.app/">https://shareyourcloning.netlify.app/</a>

<div class="img-wrapper">
    <img width="25%" src="qr_app.png" alt="">
</div>

<div class="img-wrapper">
    <img width="100%" src="app_screenshot.png" alt="">
</div>



</div>
</div>

<div class="box full">

# <i class="fab fa-github"></i> 🛠️ Get involved! 🛠️ <i class="fab fa-github"></i>

<div class="content centered">
<a href="https://github.com/manulera/ShareYourCloning/">https://github.com/manulera/ShareYourCloning/</a>
<div class="img-wrapper">

|Frontend repo|Backend repo|Contributing.md|
|--|--|--|
|<img width="75%" src="qr_frontend_repository.png" alt="">|<img width="75%" src="qr_backend_repository.png" alt="">|<img width="75%" src="qr_contribution.png" alt="">|

<span></span>
</div>

</div>
</div>