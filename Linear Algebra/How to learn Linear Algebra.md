## Quora [answer](https://www.quora.com/How-can-I-self-study-Linear-Algebra?top_ans=1603481) by Yan Zhang

Okay I clearly care too much about teaching linear algebra:

**I. The Two Levels of Linear Algebra

There are two levels of understanding linear algebra that I think are most relevant:

**EDIT:** I just realized how easily my advice here can be misconstrued. I want to point out that (2) is not meant to represent all "abstract" material as much as a certain pedagogical trend in teaching "advanced" linear algebra that try to avoid matrices (and sometimes even the determinant... Axler doesn't do it until Chapter 10 or something). **Thinking about matrices and vectors as abstract objects and introducing the notion of "vector space" etc. still count as (1) and is actually done in, say, Strang's books/lectures, and is definitely part of the fundamentals.** I make this contrast mainly to combat the idea that somehow "if you are smart, you should just do Linear Algebra Done Right and never think about matrices," which I think is a trap for "intelligent" beginners. I **do** think the abstraction of vector spaces are valuable, even for (1). I apologize for this confusion and have changed my wording slightly.

1) using matrices as the focus. This is the Strang school, which advocates that the best method is to play with matrices through concrete calculations. For this, Strang's lecture notes at the MIT OCW is agreed by many to be the best resource (opinions on his book are more mixed, but I personally still think they are useful). If you see linear algebra as **a tool you want to use** instead of **a story you want to learn**. I'd highly advise you stop here and just learn to use the tool in actual computations. If you are slightly more ambitious, maybe get some projects involving MATLAB, Mathematica, Maple, or SAGE. Seeing actual numbers helps a lot. This is why people like Alan Edelman are ridiculous with matrices.

2) using abstract linear algebra as the focus. This is the "Linear Algebra Done Right" approach which I think is horrible if you just want to learn it as a tool. For, say, a math graduate student, this becomes indispensable (however, most people we teach don't become graduate students, a fact that we mathematicians are horrible at remembering). Axler's book is pretty good at this, but a gem that I don't see recommended enough is Paul Halmos' The Linear Algebra Problem Book. While people should really just read anything by Paul Halmos, I found this collection particularly helpful and enjoyable. As a bonus, I think even people who are only interested in (1) can gain a fair bit from this book.

I think unless you have some talent, skipping to (2) directly, even if you understand it, does not make you good at (1). It's been said (I'm taking slight liberty) that the best mathematicians will refuse to acknowledge rows and columns of numbers, but when the night has come and the land is dark and their parents aren't looking, they are in their offices secretly struggling to multiply matrices (and often getting it wrong). For most of the world that uses math (that is: not mathematicians), learning (1) solidly and doing (2) as fun/inspiration seems to be the best and the most painless way to go. If you do this, be proud that you are learning Linear Algebra Done Wrong, because it is still linear algebra and it still is awesome.

-------

II. The Mental Preparation for Linear Algebra

Another thing that I really want to mention is that linear algebra is a pretty big meal for most newcomers, so having "guiding principles" in your mind as you learn it will speed up the process. Here are the 3 that I found most useful for my students and for myself:

1) keep a list of "equivalent things" to invertibility. You'll realize that a lot of concepts neatly focus this way, from eigenvalues to solving equations to rank to taking matrix inverses. People who are experienced do these things fairly automatically, but it may take some time to get used to this if you are new.

2) always always think about how to take the "skeleton" of a matrix that captures most of its essence. The clearest example of this is a dirty secret: mathematicians (and especially physicists) like to "squint their eye" at a matrix and only see a diagonal matrix with the eigenvalues on the diagonal, then they make smart-sounding statements about the matrix and then justify it later with similarity transformations and (heaven forbid) the Jordan form.

3) (slightly more relevant for abstract thinking, but useful for both) matrices always have two interpretations: one as a transformation that eats vectors and spits out vectors; the other as a bilinear form that eats two vectors and spits out a number. To kill your confusion by 80%, always mentally remind yourself which world you are in. This also helps you to remember when you need to wrap your matrix by something and its inverse (the former) and when you need to wrap your matrix by something and its transpose (the latter).

----  
III. The Application of Linear Algebra

This is for learning a course in linear algebra. Of course, there is also how to see linear algebra in the rest of the world, which to me is an important part of it (but hey, if you really just care about the course, stop reading. Your own loss). For this, I see two main things:

1) look for a matrix. Anytime there is a transformation, like a projection, there is a matrix. Let's go one step further: anytime you have independent variables, you can think of them as "transforming" into dependent variables. If you go Occam's razor and assume this is linear (most things are, or can be estimated), you have a transformation! I think this (having independent and dependent variables) is the number one reason linear algebra comes up in science. I really wished someone told me this earlier so I'm saying it now. A lot of machine learning, econometrics, and statistics really come down to just this (except ML calls variables "features" to be snoots).  
2) the single most application-worthy part of linear algebra is principal-component analysis, also known as a million other names as every field rediscovers it and puts their own name on it. The toy example I have in my head is when you have a lot of points on a 2-D plot that falls in one line - don't you really want to think of it as a line in one dimension? Congrats, you've discovered 1-d principal component analysis (or linear regression; I don't think of the two as much different =D).

Safe winds.