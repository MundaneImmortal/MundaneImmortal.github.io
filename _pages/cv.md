---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}
\documentclass[A4,11pt]{article}
% \documentclass[letterpaper,11pt]{article} %For use in US
\usepackage{latexsym}
\usepackage[empty]{fullpage}
\usepackage{titlesec}
\usepackage{marvosym}
\usepackage[usenames,dvipsnames]{color}
\usepackage{verbatim}
\usepackage{enumitem}
\usepackage[hidelinks]{hyperref}
\usepackage[english]{babel}
\usepackage{tabularx}
\usepackage{tikz}
\usepackage{float} 
\input{glyphtounicode}

%-----FONT OPTIONS-------------------------------------------------------------
\begin{comment}
The font of the document will impact not just how readable it is, but how it is
perceived. In the "The Craft of Scientific Writing" by Michael Alley, shares a
common fonts for publication as well as their use. I have chosen to use
Palatino for its legibility, some others are given below. There is far too much
about typography to discus here. Note: serif fonts have short projecting
strokes, sans-serif fonts are sans (without) these strokes.
\end{comment}


% serif
\usepackage{palatino}
% \usepackage{times} %This is the default as well
% \usepackage{charter}

% sans-serif
% \usepackage{helvet}
% \usepackage[sfdefault]{noto-sans}
% \usepackage[default]{sourcesanspro}

%-----PAGE SETUP---------------------------------------------------------------

% Adjust margins
\addtolength{\oddsidemargin}{-1cm}
\addtolength{\evensidemargin}{-1cm}
\addtolength{\textwidth}{2cm}
\addtolength{\topmargin}{-1cm}
\addtolength{\textheight}{2cm}

% Margins for US Letter size
%\addtolength{\oddsidemargin}{-0.5in}
%\addtolength{\evensidemargin}{-0.5in}
%\addtolength{\textwidth}{1in}
%\addtolength{\topmargin}{-.5in}
%\addtolength{\textheight}{1.0in}

\urlstyle{same}

\raggedbottom
\raggedright
\setlength{\tabcolsep}{0cm}

% Sections formatting
\titleformat{\section}{
  \vspace{-4pt}\scshape\raggedright\large
}{}{0em}{}[\color{black}\titlerule \vspace{-5pt}]

% Ensure that .pdf is machine readable/ATS parsable
\pdfgentounicode=1

%-----CUSTOM COMMANDS FOR FORMATTING SECTIONS----------------------------------
\newcommand{\CVItem}[1]{
  \item\small{
    {#1 \vspace{-2pt}}
  }
}

\newcommand{\CVSubheading}[4]{
  \vspace{-2pt}\item
    \begin{tabular*}{0.97\textwidth}[t]{l@{\extracolsep{\fill}}r}
      \textbf{#1} & #2 \\
      \small#3 & \small #4 \\
    \end{tabular*}\vspace{-7pt}
}

\newcommand{\CVSubheadings}[2]{
    \item
    \begin{tabular*}{0.97\textwidth}[t]{l@{\extracolsep{\fill}}r}
      #1 & #2 \\
    \end{tabular*}\vspace{-7pt}
}

\newcommand{\CVSubSubheading}[2]{
    \item
    \begin{tabular*}{0.97\textwidth}{l@{\extracolsep{\fill}}r}
      \text{\small#1} & \text{\small #2} \\
    \end{tabular*}\vspace{-7pt}
}

\newcommand{\CVSubItem}[1]{\CVItem{#1}\vspace{-4pt}}

\renewcommand\labelitemii{$\vcenter{\hbox{\tiny$\bullet$}}$}

\newcommand{\CVSubHeadingListStart}{\begin{itemize}[leftmargin=0.5cm, label={}]}
% \newcommand{\resumeSubHeadingListStart}{\begin{itemize}[leftmargin=0.15in, label={}]} % Uncomment for US
\newcommand{\CVSubHeadingListEnd}{\end{itemize}}
\newcommand{\CVItemListStart}{\begin{itemize}}
\newcommand{\CVItemListEnd}{\end{itemize}\vspace{-5pt}}

%------------------------------------------------------------------------------
% CV STARTS HERE  %
%------------------------------------------------------------------------------
\begin{document}

%-----HEADING------------------------------------------------------------------
\begin{comment}
In Europe it is common to include a picture of ones self in the CV. Select
which heading appropriate for the document you are creating.
\end{comment}

\begin{minipage}[c]{0.05\textwidth}
    \-\
\end{minipage}
% \begin{minipage}[c]{0.2\textwidth}
%     \begin{tikzpicture}
%         \clip (0,0) circle (1.75cm);
%         \node at (0,-.7) {\includegraphics[width = 4.5cm]{lzlh_new}};
%         % if necessary the picture may be moved by changing the at (coordinates)
%         % width defines the 'zoom' of the picture
%     \end{tikzpicture}
%     \hfill\vline\hfill
% \end{minipage}
\begin{minipage}[c]{\textwidth}
  \begin{flushleft}
    \textbf{\Huge \scshape{Jiazhen Xu}} \\ \vspace{2pt}
    \small{Icon, 213 E Springfield Ave, Urbana, IL 61820} \\
    Email: \href{mailto:jiazhen6@illinois.edu}{{\color{blue}jiazhen6@illinois.edu}} 
    % $|$ Website: \href{https://zilinghan.github.io}{\color{blue}Zilinghan.github.io} 
    $|$
    \small{(+86) 151-3218-1124 $|$ (+1) 217-904-2831}
    % \href{mailto:Zilinghan.18@intl.zju.edu.cn}{{Zilinghan.18@intl.zju.edu.cn}} \quad
  \end{flushleft}
  \begin{picture}(50,50)(0,0)
    \put(470,60){\includegraphics[scale=0.05]{photo.jpg}}
   \end{picture} 
   \vspace{-70pt}
\end{minipage}

\begin{comment}
This CV was written for specifically for positions I was applying for in
academia, and then modified to be a template.

A standard CV is about two pages long where as a resume in the US is one page.
sections can be added and removed here with this in mind. In my experience,
education, and applicable work experience and skills are the most import things
to include on a resume. For a CV the Europass CV suggests the categories: Work
Experience, Education and Training, Language Skills, Digital Skills,
Communication and Interpersonal Skills, Conferences and Seminars, Creative Works
Driver's License, Hobbies and Interests, Honors and Awards, Management and
Leadership Skills, Networks and Memberships, Organizational Skills, Projects,
Publications, Recommendations, Social and Political Activities, Volunteering.

Your goal is to convey a who, what , when, where, why for every item you share.
The who is obviously you, but I believe the rest should be done in that order.
For example below. An employer cares most about the degree held and typically
less about the institution or where it is located (This is still good
information though). Whatever order you choose be consistent throughout.
\end{comment}

\section{Self-Introduction}
    I’m \textbf{self-motivated} and \textbf{determined} with a strong desire for a \textbf{PHD} degree in \textbf{Computer Science}. I firmly believe that ardent love brings me invincible faith to fulfil every choice and commitment. Coding, music, and sports, the three major components of my life, are really where my passion lies. Besides, I am always prepared to explore possibilities instead of staying at my comfort zone.

%-----EDUCATION----------------------------------------------------------------
\section{Education}
\CVSubHeadingListStart
%    \CVSubheading % Example
%      {Degree Achieved}{Years of Study}
%      {Institution of Study}{Where it is located}
\CVSubheading
{{Zhejiang University \& University of Illinois at Urbana–Champaign}}{Sep. 2019 -- Jun. 2023}
{Bachelor of Science in Computer Engineering (double degree)}{\textbf{CGPA: 3.90/4.0}}
\CVSubheadings
{\textbf{Exchange at University of Illinois at Urbana-Champaign  }}{Jan. 2022 -- Jun. 2022}
% \CVSubheading
% {{University of Illinois at Urbana–Champaign}}{Sep. 2018 -- May. 2022}
% {Bachelor of Science in Computer Engineering (double degree)}{GPA: 3.95/4.0} Engineering in Electronic and Computer Engineering
% \CVSubheading)
% {{Bachelor of Arts $|$ \emph{\small{Major: Physics, Minor: Education}}}}{Aug. 2016 -- May 2018}
% {Austin College}{Sherman, TX}
% \CVSubheading
% {Associate of Liberal Sciences}{Aug. 2015 -- May 2016}
% {North Lake College}{Irving, TX}
\CVSubHeadingListEnd

%-----PUBLICATIONS------------------------
\section{Publications}
\CVSubHeadingListStart
%    \CVSubheading
%      {Title of Work}{When it was done}
%      {Institution you worked with}{unused}
% \CVSubheading
% {Conference Paper}{}
%   {\textbf{[Pub1] }\textbf{Li Z.}, He S., Du Y., González S., Schewe KD. Unbounded Barrier-Synchronized Concurrent ASMs for Effective\\ MapReduce Processing on Streams. In \textit{Rigorous State-Based Methods. ABZ 2021.}  Lecture Notes in Computer\\Science, vol 12709.  Springer, Cham. \href{https://doi.org/10.1007/978-3-030-77543-8_1}{\underline{\textbf{[Paper]}}}}{}

% \CVSubheading
% {{Unbounded Barrier-Synchronized Concurrent ASMs} $|$ \emph{\small{C++}}}{May 2020 - Feb. 2021}
% {Advisor: Prof. Klaus-Dieter Schewe (Full paper as first author, accepted by \href{https://abz2021.uni-ulm.de/}{\underline{ABZ2021}})}{}

\CVSubheading
{Preprint Paper}{}
  {%   \textbf{[Pub2] }Yuan X.$^*$, \textbf{Li Z.}$^*$, Wang G. ActiveMatch: End-to-end Semi-supervised Active Representation Learning, Submi-\\-tted to \textit{ICASSP 2022}. ($^*$: equal contributions) \href{https://arxiv.org/pdf/2110.02521.pdf}{\underline{\textbf{[Paper]}} }\\
\textbf{[Pub1]} Hu W., Liu Y., \textbf{Xu J.}, Chen X., Wang G.  Learn Discrimination From Contaminated Data: Multi-Instance Learning \\ With Convex Representation for Unsupervised Anomaly Detection. Submitted to \textit{ICME 2022}.
  }{}
% {{FPGA based Game Design: Fruit Ninja} $|$ \emph{\small{System Verilog}}}{Nov. 2020 - Dec. 2020}
% {Advisor: Prof. Chushan Li (Final project design of ECE385)}{}
% \CVSubheading
% {{Unbounded Barrier-Synchronized Concurrent ASMs} $|$ \emph{\small{C++}}}{May 2020 - Feb. 2021}
% {Advisor: Prof. Klaus-Dieter Schewe (Full paper as first author, accepted by \href{https://abz2021.uni-ulm.de/}{\underline{ABZ2021}})}{}

\CVSubHeadingListEnd


%-----WORK EXPERIENCE----------------------------------------------------------
\begin{comment}
try to briefly explain what you did and why it is relevant to the position you
are seeking
\end{comment}

% \section{Work Experience}
% \CVSubHeadingListStart
% %    \CVSubheading %Example
% %      {What you did}{When you worked there}
% %      {Who you worked for}{Where they are located}
% %      \CVItemListStart
% %        \CVItem{Why it is important to this employer}
% %      \CVItemListEnd
% \CVSubheading
% {Integration Engineering Intern}{June 2018 -- August 2019}
% {Finisar Corp.}{Sherman, TX}
% \CVItemListStart
% \CVItem{Worked in ISO 4 cleanroom developing applications to improve efficiency and creating specs}
% \CVItem{Employed metrology and microscopy for failure analysis and developing process for wet etching}
% \CVItem{Member of Emergency Response Team}
% \CVItemListEnd
% \CVSubheading
% {Laboratory Assistant}{January 2016 -- July 2016}
% {North Lake College}{Irving, TX}
% \CVItemListStart
% \CVItem{Inventoried and maintained Physics Department lab equipment}
% \CVItem{Physics tutoring}
% \CVItemListEnd
% \CVSubheading
% {Assistant Manager}{December 2006 -- August 2015}
% {Sun \& Ski Sports}{Austin, TX}
% \CVItemListStart
% \CVItem{Led a team of 20+ employees}
% \CVItem{Ran social media, as well as all grassroots marketing}
% \CVItemListEnd
% \CVSubHeadingListEnd

%-----PROJECTS AND RESEARCH----------------------------------------------------
\begin{comment}
Ideally the title of the work should speak for what it is. However if you feel
like you should explain more about why the project is applicable to this job,
use item list as is shown in the work experience section.
\end{comment}

\section{Selected Projects and Research}
\CVSubHeadingListStart
%    \CVSubheading
%      {Title of Work}{When it was done}
%      {Institution you worked with}{unused}
% \CVSubheading
% {Movie Characters Recognition using Deep Learning $|$ \emph{\small{Python}}}{Sep. 2021 - Present}
% {Advisor: Prof. Volodymyr Kindratenko, University of Illinois at Urbana–Champaign}{}
% \CVItemListStart
% \CVItem{Built a deep learning network that can return the time slots in which each main character appears. The model can serve as a handy tool for generating statistical data to assist movie analysis.}
% \CVItem{Applied the semi-supervised learning method to train the face recognition network to fully leverage the unlabeled images from movies and reduce the required number of labeled images.}
% \CVItemListEnd

\CVSubheading
{Multi-Instance Learning for Unsupervised Anomaly Detection. [Pub1] $|$ \emph{\small{Python}}}{Jun. 2021 - Sep. 2021}
{Advisor: Prof. Gaoang Wang, Zhejiang University}{}
\CVItemListStart
% \CVItem{Submitted a paper as the joint first author to \textit{2022 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)}. \href{https://arxiv.org/pdf/2110.02521.pdf}{\textbf{[Paper]}}}
\CVItem{Propsed anomaly discrimination learning with pseudo normality score generation and multi-instance contrastive learning for distinguishing abnormal samples from the unlabeled set.}
\CVItem{Combined the discrimination learning with mean-shifted contrastive learning and distribution-shifting transformation classification into a multitask representation learning framework to improve the stability and robustness of the training.}
\CVItemListEnd


% \CVSubheading
% {{A Scalable and Extendible Generative Adversarial Imputation Toolbox [Pub3]}}{Jun. 2021 - Sep. 2021}
% {Advisor: Prof. Xiaoye Miao, Zhejiang University}{}
% \CVItemListStart
% \CVItem{Proposed an improved generative adversarial network (GAN) based missing data imputation method. It solved the problem of vanishing gradient and speeded up the model training by \textbf{7.5x} on average.}
% \CVItem{Built an imputation toolbox with the GAN-based model embedded, which can serve as a powerful GUI tool for data scientists to upload, merge, preprocess and impute their datasets.}
% % \CVItem{\textsf{SCIS} can train imputation models constructed by GAN via using an appropriate sample size under accuracy guarantees for large-scale incomplete data, and can speed up model training by \textbf{7.5x} on average.}
% \CVItemListEnd



% \CVSubheading
% {{Unbounded Barrier-Synchronized Concurrent ASMs [Pub1]} $|$ \emph{\small{C++}} }{May. 2020 - May. 2021}
% {Advisor: Prof. Klaus-Dieter Schewe, Zhejiang University}{}
% \CVItemListStart
% % \CVItem{Published a full paper as the first author on \href{https://abz2021.uni-ulm.de/}{{ABZ2021}}. \href{https://doi.org/10.1007/978-3-030-77543-8_1}{\textbf{[Paper]}}}
% \CVItem{Based on the bulk-synchronous parallel (BSP) model, extended the normal MapReduce algorithm from processing large finite datasets to processing stream queries with input data assumed to continue indefinitely.}
% % \CVItem{Divided stream queries into three classes: memoryless, semi-memoryless and memorable, and provided the MapReduce implementations for each class based on the BSP model.}
% \CVItem{Extended the BSP model to the Infinite-Agent BSP model capturing an unbounded number of agents. A behavioral theory was developed for the extended model as well.}
% \CVItemListEnd


% \CVSubheading
% {{Linux-like Operating System Supporting Multiple Terminals} $|$ \emph{\small{C, x86-Assembly}}}{Mar. 2021 - May 2021}
% {Advisor: Prof. Lumetta and Kalbarczyk, University of Illinois at Urbana–Champaign}{}
% \CVItemListStart
% \CVItem{Developed a Linux-like operating system using C and x86 Assembly with three other students from scratch.}
% \CVItem{In addition to basic functionalities of OS like basic device supports, interrupt handlers, multiple shells and schedulers, we also implemented several advanced functionalities such as dynamic memory allocation, writable file-system, random number generator, .wav file play, status bar and a simplified vim.}
% \CVItemListEnd
% \CVSubheading
% {{FPGA based Game Design: Fruit Ninja} $|$ \emph{\small{System Verilog}}}{Nov. 2020 - Dec. 2020}
% {Advisor: Prof. Chushan Li, Zhejiang University}{}
% \CVItemListStart
% \CVItem{Developed an FPGA-based game called Fruit Ninja with another classmate. It realized smooth movements of the fruits in parabolic curves with central rotations and accurate detections of the cutting processes. Our designed game won the \textbf{best design awards} for course ECE385 (Digital Systems Laboratory).}
% \CVItem{The game supported both single player mode \textbf{[\href{https://zilinghan.github.io/images/Single_Player.mp4}{Demo}]}}and double player mode \textbf{[\href{https://zilinghan.github.io/images/Double_Player.mp4}{Demo}]}.
% \CVItemListEnd
\CVSubheading
{{FPGA based Game Design: BOXHEAD3: 2 Players} $|$ \emph{\small{System Verilog}}}{Dec. 2021}
{Advisor: Prof. Chushan Li, Zhejiang University \& Prof. Zuofu Chen, UIUC (Final project design of ECE385)}{}
\CVItemListStart
\CVItem{[\href{https://github.com/MundaneImmortal/ECE385/tree/master}{Source code}]}
\CVItemListEnd
\CVSubHeadingListEnd



%-----TEACHING EXPERIENCE------------------------------------------------------
\begin{comment}
Section is here as it applied to my application for positions in academia.
Remember to tailor the resume for to the position.
\end{comment}

%-----HONORS AND AWARDS--------------------------------------------------------
\section{Selected Honors and Awards}
\CVSubHeadingListStart
%    \CVSubheading %Example
%      {What}{When}
%      {Short Description}{}
% \CVSubheading
% {Provincial Government Scholarship of Zhejiang Province}{2021}
% {Top $3\%$ university students in Zhejiang province}{}
% \CVSubheading
% {National Scholarship}{2020}
% {$0.2\%$ of Chinese university students get this award}{}
% \CVSubheading
% {Zhejiang University Scholarship - First Prize}{2020}
% {Top $3\%$ students in Zhejiang University}{}
\CVSubheading
{Zhejiang University Scholarship - Second Prize}{2021}
{Top $8\%$ students in Zhejiang University}{}
\CVSubheading
{Mathematical Competition of Senior High School of China - First Prize} {2018}
{Ranking of 21 in Heibei Province}{}
\CVSubHeadingListEnd

%-----SKILLS-------------------------------------------------------------------
\begin{comment}
This section is compressed from the various skills sections that Euro CV
recommends.
\end{comment}

\section{Skills}
\begin{itemize}[leftmargin=0.5cm, label={}]
    \small{\item{
          \textbf{Programming Languages}{: Python, C, C++, System Verilog}\\ \vspace{4pt}
          \textbf{Tools}{: PyTorch, CUDA} \\
          }}
        %   \textbf{Languages}{: Mandarin, English (\textbf{TOEFL: 112} Listening: 30, Reading: 29, Writing: 29, Speaking: 24)}
        %   }}
\end{itemize}

\section{Teaching Assistant Experience}
\begin{itemize}[leftmargin=0.5cm, label={}]
    \small{\item{
          \textbf{Math 241 (Calculus \uppercase\expandafter{\romannumeral3})}{: Basic Linear Algebra, Vector Functions, Multivariate Calculus, Vector Fields} \\
          }}
\end{itemize}


% \section{English Skills}
% \begin{itemize}[leftmargin=0.5cm, label={}]
%   \small{\item{
%         \textbf{TOEFL (112)}{ Listening: 30, Reading: 29, Writing: 29, Speaking: 24}\\
%         \textbf{GRE (324+3.5)}{ Verbal: 156, Quantitative: 168, Writing: 3.5}
%         }}
% \end{itemize}

%-----CONFERENCES AND PRESENTATIONS--------------------------------------------
\begin{comment}
Again the title should have already been enough, but if it is necessary to add
descriptions maintain the consistency from prior sections
\end{comment}

% \section{Conferences and Presentations}
% \CVSubHeadingListStart
% %    \CVSubheading % Example
% %      {Work Presented}{When}
% %      {Occasion}{}
% \CVSubheading
% {Photometric Filter Fidelity and Use for Be Star Identification}{November 2017}
% {Austin College Physics Research Seminar}{}
% \CVSubheading
% {Reflectometry for Volumetric Soil Moisture Measurement}{May 2017}
% {Austin College Atmospheric Physics Fair}{}
% \CVSubheading
% {Design and Manufacturing of Products using 3D Printing}{April 2017}
% {Austin College Student Scholarship Conference}{}
% \CVSubHeadingListEnd


\section{Extracurricular Activities}
% \begin{itemize}[lftmargin=0cm, label={}]
%     \small{\item{
          \CVSubHeadingListStart
          \CVSubheadings
          {\textbf{Champion} of Zhejiang University International Campus Football Cup as the \textbf{captain}} {2020, 2021}\\
          \CVSubheadings
          {\textbf{Golden Shoe winner} of Zhejiang University International Campus Football Cup}{2020, 2021}\\
          \CVSubheadings
          {\textbf{Silver Medalist} of mixed doubles in Zhejiang University International Campus Badminton Cup}{2019}\\
          \CVSubheadings
          {\textbf{Bronze Medalist} of men's 110 m hurdle at Zhejiang University Sports Meeting}{2021}
          \CVSubHeadingListEnd
          %}}
% \end{itemize}

\section{Selected Courses}
I get A/A+ in all 13 major courses since my sophomore year! Some of them are listed:
\CVSubHeadingListStart
\CVSubheading
{ECE 374}{A+}
{Intro to Algorithms and Models of Computing}{}
\CVSubheading
{ECE 385}{A+}
{Digital Systems Laboratory}{}
\CVSubheading
{CS 225}{A+}
{Data Structure}{}
\CVSubheading
{Math 213}{A+}
{Discrete Mathematics}{}
\CVSubheading
{ECE 408}{A}
{Parallel Programming}{}
\CVSubheading
{ECE 220}{A}
{Computer Systems and Programmings}{}
\CVSubheading
{ECE 313}{A}
{Probability with Engineering Applications}{}
\CVSubheading
{Math 286}{A}
{Differential Equation Plus}{}
\CVSubheading
{Math 241}{A}
{Calculus \uppercase\expandafter{\romannumeral3}}{}

\CVSubHeadingListEnd

%------------------------------------------------------------------------------
\end{document}