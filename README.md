# About

This project objective is implementing an agent that can act properly
in the Pole Balancing controle problem defined in:

https://webdocs.cs.ualberta.ca/~sutton/papers/barto-sutton-anderson-83.pdf

OpenAi provided the actual environment:

https://gym.openai.com/envs/CartPole-v0

# Python dependencies

First, the usual:

- numpy
- pandas
- matplotlib
- jupyter

Now, the specific stuff that I used:

- gym: provides the CartPole environment from OpenAI.
- Keras: the neural network library.
- Theano or TensorFlow: keras uses one of them internally.
- h5py: saves and loads data.
- tqdm: progress bar library.
- Seaborn: creates beautiful visualizations (or so I've been told)

# Running the code

The notebook file capstone.ipynb includes all the source code. As for
the report, I had all texlive packages installed; to compile it, run:

$ cd report
$ pdflatex report.tex; bibtex report; pdflatex report.tex; pdflatex report.tex;

(No need to compile, though: just open the file report.pdf)

# Additional comments

All coding and testing were done in Linux and I had to install the
following packages:

- cmake
- zlib1g-dev

I have run into some problems to render the OpenAI environment (mostly
opengl errors in a computer without a proper discrete graphics card;
in my main computer, everything runned smoothly). To check if opengl
is working well, try opening glxgears.
