# Syllabus for CS 6831

Welcome to CS 6831, Designing Secure Cryptography. We will be learning about
the modern theory and practice of the cryptographic tools deployed to protect
contemporary computing systems. In addition to learning more about the types of
cryptographic tools currently used, we will be focusing on understanding the
processes that, ideally, lead to secure tools.  Topics include formulation of
security definitions, reduction-based concrete security analysis, evaluation of
real-world implementations, common pitfalls, and attacks. Active research topics
will be highlighted throughout. 


Instructor: Tom Ristenpart (https://rist.tech.cornell.edu)

Time: 1:55pm-3:10pm M/W

NYC classroom: Bloomberg 091

Ithaca classroom: Gates 405

### Pre-requisites

By the end of the class you should have the ability to design and argue the
security of new cryptographic tools, at the level of quality of new publishable
research results. This will be a fast-paced course.

Students will be expected to have taken courses or otherwise have substantial
background on computer security; have knowledge of basic cryptographic concepts
(encryption, hashing); and experience doing formal math (proofs, etc.).  

The class is for PhD students, and will assume a lot of shared background
material. Cornell Tech masters students should only consider the class if they
are comfortable with probability theory, discrete mathematics, computational
complexity, and computer security.  You might refer to the Bellare-Rogaway
notes, Section 1.5.  For a taste of what they mean by mathematical maturity,
refer to the Boneh-Shoup book Section 2.4. If that material doesn't look
familiar, or you spent a lot of time struggling to understand it, then that may
suggest you'll have a hard time getting much out of the class.  The first time I
took a PhD class of this form, I spent innumerable hours a week on it, and had
the freedom to do so as a PhD student with few other responsibilities. 

It is really important to note that this does not mean *you are not capable of
mastering cryptography*, and I don't want to discourage you from the field.
Rather, there's a bit of a jargon and concept barrier that must be filled in,
and doing so would unfairly sacrifice content from the PhD students.  Usually we
teach a masters level course that covers a subset of this material at a more
suitable pace, but unfortunately that's not possible this year. 

With that set of warnings in place, Cornell Tech students should talk to me if
they want to take the class after the first lecture.  Be prepared to answer some
questions about your understanding of Boneh-Shoup Section 2.4.


### Requirements

The class will involve two main deliverables. One will be scribe notes. The goal
will be to have a complete set of notes for future reference. We will figure out
early on the scribing schedule. Each student will be responsible for
delivering one or more complete writeups of lecture topic(s).  This will notably
include finished, precise proofs that may be only covered at a high level in
class, accompanied by beautiful English prose.  See new section added below.

Second will be a semester project, the aspirational goal being a
publication-worthy result in applied cryptography. The project deliverable will
be a short report together with a one-on-one oral discussion (possibly over
Zoom) with the me about the result. A paper worked on with others can substitute
for the short report, though you will need to identify your specific
contributions.  The one-on-one discussion will allow you to gain practice
describing your work in a professional setting, allow me to assess what you've
learned from the class, and help determine your final grade. More details
will be forthcoming. 

I may also point out problems or omitted proofs that you will want to work on to
solidify your understanding of material. These will be ungraded, but I can give
you feedback if you desire. 

Grades will be assigned according to the following breakdown:

* Participation: 20%
* Scribe notes :  40% 
* Project:  40% 

### Scribing

I will send out a spreadsheet with a tentativie scribing schedule.  PhD students
will be doing scribing.  There will be one scribe and two proofreaders for each
lecture. The scribe will write up an initial draft of the notes for the lecture,
and the proofreaders will provide technical and editorial feedback before I take
a look. The scribe and proofreaders are, together, also responsible for coming
up with three self-study questions (i.e., homework problems) that speak to the
material. These should not be questions that require regurgitating something,
but rather that make people think deeply about the material.  Feel free to
borrow problems from public sources (e.g., Boneh-Shoup book), but be very clear
about attribution (even if it was just used for inspiration) and include the
attribution in the notes. 
Initial draft is due a week after lecture, and proof-read finald raft 1.5 weeks
after lecture. If there's going to be some reason for a delay, let me know.

The masters students will be responsible for testing out (a reasonable subset)
of these questions by working out candidate solutions individually. We'll group
things into ~6-lecture chunks, and assign a problem from each. So masters
students can expect 3 problem sets, finishing 3/4 of the way through the
class to minimize problem set and end-of-term project overlaps. If the problems
are too hard, we'll adjust accordingly how many students need to solve.  These
will be peer-graded by the PhD student(s) who first conceived the problem with
my oversight and final approval of grading.  The involved PhD students and
masters students will determine the worst solution, and the responsible student
will get the honor of typesetting a correct solution for inclusion in an
appendix in the notes. They can use as reference all the solutions, and work
with whomever can help them out to do so. For the masters students the 40\% of
class grade will be associated to performance on problem sets. Of course, MS
students can help out with proof-reading and embellishments to scribe notes via
pull requests (see below), and this will positively count towards your
participation and scribe grades.

I have added the notes to the git repository. You can therefore fork this
repository, work in a local copy, and then submit a pull request to me once the
notes are ready for my review. They should already be proofread by both
proofreaders before a PR comes in. Let me know if this workflow doesn't work out
for you. 

The end result should be an open-source set of notes that others can use as they
explore this topic. Everyone who finishes the class will get appropriate credit
for contributing. 

All this will require some good will and coordination among students. If anyone
has any concerns or problems, don't hesitate to talk to me.


### Background reading

One of the goals of the course will be to produce lecture notes on this content
useful for others. The following excellent references will be useful throughout the course,
particularly the Boneh-Shoup book and Bellare-Rogaway notes. 

* [A Graduate Course in Cryptography](https://crypto.stanford.edu/~dabo/cryptobook/BonehShoup_0_4.pdf).
   Boneh-Shoup book. A mixture of asymptotic and concrete security.

* [Bellare and Rogaway lecture notes](http://web.cs.ucdavis.edu/~rogaway/classes/227/spring05/book/main.pdf).
  A somewhat dated set of lecture notes. Focuses on concrete security approach.


* [Bellare lecture slides](https://cseweb.ucsd.edu/~mihir/cse207/classnotes.html). Slides from
  Mihir Bellare's graduate course in cryptography, based in large part on the notes.
  

* [Modern Cryptography by Katz and Lindell](http://www.cs.umd.edu/~jkatz/imc.html). Katz-Lindell book focuses on
 asymptotic definitions. 



## Lecture schedule

A very preliminary and aspirational schedule is below to give a taste of the scope of
what we're hoping to cover.  


| Date |  Topic  |  Slides | Notes |
|------|---------|---------|-------|
| Jan 23 | Intro |  [Slides](slides/intro-lec1.pdf) | |
| Jan 28 | Block ciphers, PRPs, PRFs | [Slides](slides/ciphers-lec2.pdf) | |
| Jan 30 | Cryptanalysis, frequency attacks |  | |
| Feb 4 |  PRGs, Block cipher modes |  | |
| Feb 6 |  Message authentication, universal hashing | | |
| Feb 11 | Authenticated encryption |  | |
| Feb 13 | Nonce-based and robust authenticated encryption |   | |
| Feb 18 | Cryptographic hashing  |  | |
| Feb 20 | Password hashing, randomness extractors |  | |
| Feb 25 | No Lecture (February break) | |
| Feb 27 | Public-key encryption |  | |
| Mar 4  | RSA PKE |  | |
| Mar 6  | Discrete log PKE  |  | |
| Mar 11 | ECC crypto  |  | |
| Mar 13 | Digital signatures | | |
| Mar 18 | Blind signatures and OPRFs  | | |
| Mar 20 | Identification protocols and Fiat-Shamir |   | |
| Mar 27 | Zero-knowledge proofs  |  | |
| Apr 1  | No lecture (Spring Break) |  | |
| Apr 3  | No lecture (Spring Break) |  | |
| Apr 8  | Key exchange | | |
| Apr 10 | TLS 1.3  | | |
| Apr 15 | Signal   | | |
| Apr 17 | Group messaging | | |
| Apr 22 | Encrypted databases | | |
| Apr 24 | TBA | | |
| Apr 29 | TBA | | |
| May 1  | TBA | | |
| May 6  | TBA |  | |

