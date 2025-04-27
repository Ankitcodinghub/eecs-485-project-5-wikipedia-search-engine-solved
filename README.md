# eecs-485-project-5-wikipedia-search-engine-solved
**TO GET THIS SOLUTION VISIT:** [EECS 485 Project 5: Wikipedia Search Engine Solved](https://www.ankitcodinghub.com/product/eecs-485-project-5-wikipedia-search-engine-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;53975&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EECS 485 Project 5: Wikipedia Search Engine Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
<h1>Introduction</h1>
Build a scalable search engine that is similar to a commercial search engine. The search engine in this assignment has several features:

Indexing implemented with MapReduce so it can scale to very large corpus sizes

Information retrieval based on both tf-idf and PageRank scores

A new search engine interface with two special features: user-driven scoring and summarization.

The learning goals of this project are information retrieval concepts like PageRank and tf-idf, parallel data processing with MapReduce, and writing an end-to-end search engine. <strong>Table of Contents</strong>

Setup

Inverted Index with MapReduce

Index server

Search interface

Deploy to AWS

Submitting and grading

FAQ

<h1>Setup</h1>
<strong>Group registration</strong>

Register your group on the <a href="https://autograder.io/">Autograder</a>.

<h2>AWS account and instance</h2>
You will use Amazon Web Services (AWS) to deploy your project. AWS account setup may take up to 24 hours, so get started now. Create an account, launch and configure the instance. Don’t deploy yet. <a href="https://eecs485staff.github.io/p2-insta485-serverside/setup_aws.html">AWS Tutorial</a><a href="https://eecs485staff.github.io/p2-insta485-serverside/setup_aws.html">.</a>

<h2>Project folder</h2>
Create a folder for this project (<a href="https://eecs485staff.github.io/p1-insta485-static/setup_os.html#create-a-folder">instructions</a><a href="https://eecs485staff.github.io/p1-insta485-static/setup_os.html#create-a-folder">)</a>. Your folder location might be different.

$ pwd

/Users/awdeorio/src/eecs485/p5-search-engine

<h2>Version control</h2>
Set up version control using the <a href="https://eecs485staff.github.io/p1-insta485-static/setup_git.html">Version control tutorial</a>.

Be sure to check out the <a href="https://eecs280staff.github.io/p1-stats/setup_git.html#version-control-for-a-team">Version control for a team</a> tutorial.

After you’re done, you should have a local repository with a “clean” status and your local repository should be connected to a remote GitLab repository.

$ pwd

/Users/awdeorio/src/eecs485/p5-search-engine

$ git status

On branch master

Your branch is up-to-date with ‘origin/master’.

nothing to commit, working tree clean

$ git remote -v

origin https://gitlab.eecs.umich.edu/awdeorio/p5-search-engine.git (fetch) origin https://gitlab.eecs.umich.edu/awdeorio/p5-search-engine.git (push) You should have a <sub>.gitignore</sub> file (<a href="https://eecs485staff.github.io/p1-insta485-static/setup_git.html#add-a-gitignore-file">instructions</a>).

$ pwd

/Users/awdeorio/src/eecs485/p5-search-engine

$ head .gitignore

This is a sample .gitignore file that’s useful for EECS 485 projects.

<em>… </em>

<h2>Python virtual environment</h2>
Create a Python virtual environment using the <a href="https://eecs485staff.github.io/p1-insta485-static/setup_virtual_env.html">Python Virtual Environment Tutorial</a>.

Check that you have a Python virtual environment, and that it’s activated (remember <sub>source </sub>env/bin/activate ).

$ pwd

/Users/awdeorio/src/eecs485/p5-search-engine

$ ls -d env env

$ echo $VIRTUAL_ENV

/Users/awdeorio/src/eecs485/p5-search-engine/env

<h2>Starter files</h2>
Download and unpack the starter files.

$ pwd

/Users/awdeorio/src/eecs485/p5-search-engine

$ wget https://eecs485staff.github.io/p5-search-engine/starter_files.tar.gz $ tar -xvzf starter_files.tar.gz

Move the starter files to your project directory and remove the original <sub>starter_files/ </sub>directory and tarball.

$ pwd

/Users/awdeorio/src/eecs485/p5-search-engine

$ mv starter_files/<strong>*</strong> .

$ rm -rf starter_files starter_files.tar.gz

This project involves very few starter files. You have learned everything you need to build this project from (almost) scratch. <strong>You are responsible for converting the starter files structure into the final structure.</strong> Each part of the spec will walk you through what we expect in terms of structure.

bin/ : As in previous projects, this is where convenience shell scripts will be located. You will

write search , index , and indexdb &nbsp;hadoop/ : MapReduce programs live here. See Inverted Index with Mapreduce and the

following Hadoop setup and example instructions for more details. &nbsp;hadoop/word_count/ : Sample MapReduce program, with input. &nbsp;hadoop/inverted_index/ : Build a pipeline of MapReduce programs in this directory. You will

write several map*.py and reduce*.py files, as well as a pipeline.sh script. index/index/ : Python code for the index server. See Index server for more details. search/search/ : Search interface app. See Search interface for more details.

Both the index server and the search server are separate Flask apps. The search server will serve a bundle.js of your react source code. The index server will be styled after the project 3 REST API. As in previous projects, both will be python packages that should have a <sub>setup.py </sub>.

At the end of this project your directory structure should look something like this:

$ tree –matchdirs -I ‘env|__pycache__’

<em>. </em>

├── bin

│&nbsp;&nbsp; ├── index

│&nbsp;&nbsp; ├── indexdb

│&nbsp;&nbsp; └── search

├── hadoop

│&nbsp;&nbsp; ├── hadoop-streaming-2.7.2.jar

│&nbsp;&nbsp; ├── inverted_index

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── input.txt

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── input_split.py

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── map0.py

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── map1.py

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── …

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── output_sample.txt

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── pipeline.sh

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── reduce0.py

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── reduce1.py

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── …

│&nbsp;&nbsp; │&nbsp;&nbsp; └── stopwords.txt

│&nbsp;&nbsp; └── word_count

│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ├── input

│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; │&nbsp;&nbsp; ├── file01

│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; │&nbsp;&nbsp; └── file02

│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ├── map.py

│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; └── reduce.py

├── index

│&nbsp;&nbsp; ├── index

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── __init__.py

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── api

│&nbsp;&nbsp; │&nbsp;&nbsp; │&nbsp;&nbsp; └── *.py

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── inverted_index.txt

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── pagerank.out

│&nbsp;&nbsp; │&nbsp;&nbsp; └── stopwords.txt

│&nbsp;&nbsp; └── setup.py

├── search

│&nbsp;&nbsp; ├── node_modules

│&nbsp;&nbsp; ├── package-lock.json

│&nbsp;&nbsp; ├── package.json

│&nbsp;&nbsp; ├── search

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── __init__.py

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── api

│&nbsp;&nbsp; │&nbsp;&nbsp; │&nbsp;&nbsp; └── *.py

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── config.py │&nbsp;&nbsp; │&nbsp;&nbsp; ├── js

│&nbsp;&nbsp; │&nbsp;&nbsp; │&nbsp;&nbsp; └── *.jsx

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── sql

│&nbsp;&nbsp; │&nbsp;&nbsp; │&nbsp;&nbsp; └── wikipedia.sql

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── static

│&nbsp;&nbsp; │&nbsp;&nbsp; │&nbsp;&nbsp; └── js

│&nbsp;&nbsp; │&nbsp;&nbsp; │&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; └── bundle.js

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── templates

│&nbsp;&nbsp; │&nbsp;&nbsp; │&nbsp;&nbsp; └── *.html

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── var

│&nbsp;&nbsp; │&nbsp;&nbsp; │&nbsp;&nbsp; └── wikipedia.sqlite3

│&nbsp;&nbsp; │&nbsp;&nbsp; └── views

│&nbsp;&nbsp; │&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; └── *.py

│&nbsp;&nbsp; ├── setup.py

│&nbsp;&nbsp; └── webpack.config.js

└── tests

<h2>Install Hadoop</h2>
Hadoop does not work on all machines. For this project, we will use a lightweight Python implementation of Hadoop. The source code is in <sub>tests/utils/hadoop.py </sub>.

$ pwd <em># Make sure you are in the root directory</em>

/Users/awdeorio/src/eecs485/p5-search-engine

$ echo $VIRTUAL_ENV <em># Check that you have a virtual environment</em>

/Users/awdeorio/src/eecs485/p5-search-engine/env

$ pip install sh <em># Install a required third party sh module </em>Collecting sh

<em>… </em>

$ pushd $VIRTUAL_ENV/bin

$ ln -sf ../../tests/utils/hadoop.py hadoop <em># Link to provided hadoop implementation</em>

$ popd

$ pwd

/Users/awdeorio/src/eecs485/p5-search-engine

$ which hadoop

/Users/awdeorio/src/eecs485/p5-search-engine/env/bin/hadoop

$ hadoop -h <em># hadoop command usage </em>usage: hadoop [-h] -D PROPERTIES -input INPUT -output OUTPUT -mapper MAPPER

-reducer REDUCER

Lightweight Hadoop work-alike.

optional arguments:

-h, –help&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; show this help message and exit&nbsp; required arguments:

-D PROPERTIES

-input INPUT

-output OUTPUT

-mapper MAPPER

-reducer REDUCER

If you want to play around with the real Hadoop, Appendix: B has the installation steps listed. However, for this project, we will be using our Python implemented version of Hadoop. You do not need to use the real Hadoop for this project.

<strong>End-to-End Testing</strong>

See the <a href="https://eecs485staff.github.io/p3-insta485-clientside/setup_endtoend_testing.html">End-to-End Testing Tutorial</a> in Project 3 to install Google Chrome and ChromeDriver.

<h2>Install script</h2>
Installing all of the tool chain requires a lot of steps! Follow the <a href="https://eecs485staff.github.io/p3-insta485-clientside/#install-script">Project 3 Tutorial</a> and write a bash script <sub>bin/install</sub> to install your app. However, we need to make some small changes from your previous install script.

This project has a different folder structure, so the server and front-end installation instruction needs to change. You will also have two backend servers running for this project, so you will need to install two different python packages.

Install back end

pip install -e index <em># index server</em> pip install -e search <em># search server</em>

Install front end

pushd search npm install . popd

If running the install script on CAEN, <sub>pip install</sub> might throw PermissionDenied errors when updating packages. To allow installation and updates of packages using pip add the following lines before the first <sub>pip install</sub> command.

Tell pip to write to a different tmp directory.

mkdir -p tmp export TMPDIR<strong>=</strong>tmp

You will also need to install the python implementation of hadoop. Add this to the end of your install script.

Install the hadoop implementation

pushd $VIRTUAL_ENV/bin

ln -sf ../../tests/utils/hadoop.py hadoop popd

<h2>“Hello World” with Hadoop</h2>
Next we will run a sample mapreduce word count program with Hadoop. This example will run on both real Hadoop and the provided lightweight Python implementation.

The example MapReduce program lives in <sub>hadoop/word_count/ </sub>. Change directory.

$ cd hadoop/word_count/

$ ls

input&nbsp; map.py&nbsp; reduce.py

The inputs live in hadoop/word_count/input/ .

$ pwd

/Users/awdeorio/src/eecs485/p5-search-engine/hadoop/word_count $ tree

<em>. </em>

├── input

│&nbsp;&nbsp; ├── file01

│&nbsp;&nbsp; └── file02

├── map.py

└── reduce.py $ cat input/file<strong>* </strong>hadoop map reduce file map&nbsp; map streaming file reduce&nbsp; map reduce is cool hadoop file system google file system

Run the Hadoop mapreduce job.

jar index/hadoop/hadoop-streaming-2.7.2.jar is required by the real Hadoop. The

provided implementation ignores this argument.

-D mapreduce.job.maps=N number of mappers

-D mapreduce.job.reduces=N number of reducers

-input DIRECTORY input directory

-output DIRECTORY output directory

–<sub>mapper FILE</sub> mapper executable

-reducer FILE reducer executable

$ hadoop \&nbsp;&nbsp; jar ../hadoop-streaming-2.7.2.jar \

-D mapreduce.job.maps<strong>=</strong>2 \

-D mapreduce.job.reduces<strong>=</strong>2 \

-input input \

-output output \

-mapper ./map.py \

-reducer ./reduce.py

Starting map stage

+ ./map.py &lt; output/hadooptmp/mapper-input/part-00000 &gt; output/hadooptmp/mapper-output/par + ./map.py &lt; output/hadooptmp/mapper-input/part-00001 &gt; output/hadooptmp/mapper-output/par Starting group stage

+ cat output/hadooptmp/mapper-output/* | sort &gt; output/hadooptmp/grouper-output/sorted.out Starting reduce stage

+ ./reduce.py &lt; output/hadooptmp/grouper-output/part-00000 &gt; output/hadooptmp/reducer-outp + ./reduce.py &lt; output/hadooptmp/grouper-output/part-00001 &gt; output/hadooptmp/reducer-outp Output directory: output

You will see an <sub>output</sub> directory created. This is where the output of the MR job lives. You are interested in all <sub>part-XXXXX</sub> files.

$ pwd

/Users/awdeorio/src/eecs485/p5-search-engine/hadoop/word_count

$ ls output/ hadooptmp&nbsp; part-00000&nbsp; part-00001

$ cat output/part-<strong>* </strong>cool 1 google 1 is 1 reduce 3 system 2 file 4

hadoop 2

map 4

streaming 1

<h1>Inverted Index with MapReduce</h1>
You will be building and using a MapReduce based indexer in order to process the large dataset for this project. You will be using Hadoop’s command line streaming interface that lets you write your indexer in the language of your choice instead of using Java (which is what Hadoop is written in). However, you are limited to using Python 3 so that the course staff can provide better support to students. <strong>In addition, all of your mappers must output both a key and a value (not just a key). Moreover, keys and values BOTH must be non-empty. If you do not need a key or a value, common practice is to emit a “1”</strong>

There is one key difference between the MapReduce discussed in class and the Hadoop streaming interface implementation: In the Java Interface (and in lecture) one instance of the reduce function was called for each intermediate key. In the streaming interface, one instance of the reduce function may receive multiple keys. <strong>However, each reduce function will receive all the values for any key it receives as input.</strong>

You will not actually run your program on hundreds of nodes; it is possible to run a MapReduce program on just one machine: your local one. However, a good MapReduce program that can run on a single node will run fine on clusters of any size. In principle, we could take your MapReduce program and use it to build an index on 100B web pages.

For this project you will create an inverted index for the documents in hadoop/inverted_index/input.txt through a series of MapReduce jobs. This inverted index will

contain the idf, term frequency, and document normalization factor as specified in the information retrieval lecture slides. The format of your inverted index must follow the format, with each data element separated by a space:

&lt;term&gt; &lt;idf&gt; &lt;doc_id_x&gt; &lt;occurrences in doc_id_x&gt; &lt;doc_id_x normalization factor before sq

A sample of the correctly formatted output for the inverted index can be found in hadoop/inverted_index/output_sample.txt . You can also use this sample output to check the

accuracy of your inverted index.

For your reference, here are the definitions of term frequency and idf:

And here is the definition for normalization factor for a document:

<h2>Splitter script</h2>
Each document has three properties: <sub>doc_id </sub>, <sub>doc_title </sub>, and <sub>doc_body </sub>. Your mapper code will be receiving input via standard in and line-by-line. As a result, the input is newline separated and each document is represented by 3 lines: 1st is the <sub>doc_id </sub>, 2nd is the <sub>doc_title </sub>, and the 3rd is the <sub>doc_body </sub>. This will allow you to read the input in your mapper function easily.

Input for Hadoop programs is an input directory, not file. As you will notice, our input is in one large file called <sub>hadoop/inverted_index/input.txt</sub> but your code runs with multiple mappers, and each mapper gets one input file. Consequently, you must write a custom Python script to break the large <sub>input.txt</sub> input file with over 3,000 documents (3 lines each) into smaller files and place these files into the <sub>hadoop/inverted_index/input</sub> directory. You can name your smaller input files however you like, as long as they are under the <sub>input/</sub> directory. <strong>Do not split the input file into one file per document; this will make your MapReduce pipeline run very slowly! We do not require a specific number of smaller input files, but ~30 is fine.</strong>

Example

$ pwd

/Users/awdeorio/src/eecs485/p5-search-engine/hadoop/inverted_index

$ ./input_split.py

Output directory: input/ $ ls -d input.txt input input/&nbsp; input.txt

At this point, you should be able to pass <sub>test_pipeline03_split_file</sub> in test_pipeline_public.py .

$ pytest -v ./tests/test_pipeline_public.py::TestPipelinePublic::test_pipeline03_split_fil

<h2>Hadoop pipeline script</h2>
This script will execute several MR jobs. The first one will be responsible for counting the number of documents in the input data. Name the mapper and reducer for this map0.py and reduce0.py, respectively. The next N jobs will be a “pipeline”, meaning that you will chain multiple jobs together such that the input of a job is the output of the previous job.

We have provided <sub>hadoop/inverted_index/pipeline.sh </sub>, which has helpful comments for getting started.

<h3>Job 0</h3>
The first MapReduce job that you will create counts the total number of documents. This should be run with as many mapper workers as input files and only <strong>ONE</strong> reducer worker. The mapper and reducer executables should be named <sub>map0.py</sub> and <sub>reduce0.py </sub>, respectively. The reducer should save the total number of documents in a file called <sub>total_document_count.txt </sub>. The only data in this file will be an integer representing the total document count. The total_document_count.txt file should be created in whichever directory the pipeline is executed

from.

$ pwd

/Users/awdeorio/src/eecs485/p5-search-engine/hadoop/inverted_index

$ ./pipeline.sh

<em>… </em>

Output directory: output

$ cat total_document_count.txt

3268

<h3>MapReduce pipeline</h3>
You will be going from large datasets to an inverted index, which involves calculating quite a few values for each word. As a result, you will need to write several MapReduce jobs and run them in a pipeline to be able to generate the inverted index. The first MapReduce job in this pipeline will get input from <sub>input/</sub> and write its output to <sub>output/ </sub>. The starter file <sub>pipeline.sh</sub> shows how to pipe the output from one MapReduce job into the next one.

To test your MapReduce program, we recommend that you make a new test file, with only 10-20 of the documents from the original large file. Once you know that your program works with a single input file, try breaking the input into more files, and using more mappers.

Each of your MapReduce jobs in this pipeline should have mappers and reducers equal to the number of your input files. However, your code should still work when the number of input files and correspondingly the number of mappers is changed. You may only use maximum of 9 MapReduce jobs in this pipeline (but the inverted index can be produced in fewer). The first job in the pipeline (the document counter) must have mapper and reducer executables named

map0.py , reduce0.py respectively, and the second job should be map1.py , reduce1.py , etc.

The format of your inverted index must follow the format, with each data element separated by a space: word -&gt; idf -&gt; doc_id -&gt; number of occurrences in doc_id -&gt; doc_id’s normalization factor (before sqrt)

Sample of formatted output can be found in hadoop/inverted_index/output_sample.txt . The order of words in the inverted index does not matter. If a word appears in more than one doc it does not matter which doc_id comes first in the inverted index. Note that the log for idf is computed with base 10 and that some of your decimals may be slightly off due to rounding errors. In general, you should be within 5% of these sample output decimals.

When building the inverted index file, you should use a list of predefined stopwords to remove words that are so common that they do not add anything to search quality (“and”, “the”, etc). We have given you a list of stopwords to use in hadoop/inverted_index/stopwords.txt .

When creating your index you should treat capital and lowercase letters as the same (case insensitive). You should also only include alphanumeric words in your index and ignore any other symbols. If a word contains a symbol, simply remove it from the string. Do this with the following code snippet:

<strong>import</strong> re

re<strong>.</strong>sub(r'[^a-zA-Z0-9]+’, ”, word)

You should remove non-alphanumeric characters before you remove stopwords. Your inverted index should include both <sub>doc_title</sub> and <sub>doc_body</sub> for each document.

To construct the inverted index file used by the index server, concatenate all the files in the output directory from the final MapReduce job, and put them into a new file. Make sure to copy any updated inverted index file to your index Flask app ( <sub>index/index </sub>). This can either be done at the end of the pipeline.sh or run manually after the ouput files are created.

$ pwd

/Users/awdeorio/src/eecs485/p5-search-engine/hadoop/inverted_index cat output/* &gt; inverted_index.txt

<h3>MapReduce specifications</h3>
There are a few things you must ensure to get your mappers and reducers playing nicely with both hadoop and our autograder. Here is the list:

Emit both keys <strong>and</strong> values from all mappers.

Do not emit empty keys <strong>or</strong> values.

Split key value pairs using a tab. It should be as such “key\tvalue”

Please have a newline at the end of each of your mapper and reducer outputs at <strong>every stage</strong>

Your map-reduce output must emit more than a single line.

Sample input.

1

The Document: A

This document is about Mike Bostock. He made d3.js and he’s really cool 2

The Document: B

Another flaw in the human character is that everybody wants to build and nobody wants to d

3

Document C:

Originality is the fine art of remembering what you hear but forgetting where you heard it

Sample output.

character 0.47712125471966244 2 1 1.593512841936855 maintenance 0.47712125471966244 2 1 1.593512841936855 mike 0.47712125471966244 1 1 1.138223458526325 kurt 0.47712125471966244 2 1 1.593512841936855 peter 0.47712125471966244 3 1 2.048802225347385 flaw 0.47712125471966244 2 1 1.593512841936855 heard 0.47712125471966244 3 1 2.048802225347385 cool 0.47712125471966244 1 1 1.138223458526325 remembering 0.47712125471966244 3 1 2.048802225347385 laurence 0.47712125471966244 3 1 2.048802225347385 d3js 0.47712125471966244 1 1 1.138223458526325 made 0.47712125471966244 1 1 1.138223458526325 build 0.47712125471966244 2 1 1.593512841936855 document 0.0 2 1 1.593512841936855 3 1 2.048802225347385 1 2 1.138223458526325 originality 0.47712125471966244 3 1 2.048802225347385 bostock 0.47712125471966244 1 1 1.138223458526325 forgetting 0.47712125471966244 3 1 2.048802225347385 hear 0.47712125471966244 3 1 2.048802225347385 art 0.47712125471966244 3 1 2.048802225347385 human 0.47712125471966244 2 1 1.593512841936855 fine 0.47712125471966244 3 1 2.048802225347385 vonnegut 0.47712125471966244 2 1 1.593512841936855

<h3>Common problems</h3>
Your map and reduce programs should use relative paths when opening an input file. For example, to access stopwords.txt :

<strong>with</strong> open(“stopwords.txt”, “r”) <strong>as</strong> stopwords:&nbsp;&nbsp;&nbsp;&nbsp; <strong>for</strong> line <strong>in</strong> stopwords:

<em># Do something with line </em>

<h3>Testing</h3>
Once you have implemented your MapReduce pipeline to create the inverted index, you should be able to pass all tests in test_doc_counts_public.py and test_pipeline_public.py .

$ pytest -v tests/test_doc_counts_public.py tests/test_pipeline_public.py

<h1>Index server</h1>
The index server is a separate service from the search interface that handles search queries and returns a list of relevant results. Your index server is a RESTful API that returns search results in JSON format that the search server processes to display results to the user.

<h2>Directory structure</h2>
In this project since you have two servers, the index server and the search server, you will need separate directories for each of your server applications. Your index server code is going to be inside the directory <sub>index/index</sub> and your <sub>setup.py</sub> is going to be inside the directory <sub>index </sub>. This is to allow you to use python packages with two different servers in the same project root directory. Note that the <sub>setup.py</sub> is always in a directory above the directory in which your application’s code is. Below is an example of what your final index directory structure should look like.

$ pwd

/Users/awdeorio/src/eecs485/p5-search-engine

$ tree index index/

├── index

│&nbsp;&nbsp; ├── __init__.py

│&nbsp;&nbsp; ├── api

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── __init__.py

│&nbsp;&nbsp; │&nbsp;&nbsp; └── *.py

│&nbsp;&nbsp; ├── inverted_index.txt

│&nbsp;&nbsp; ├── pagerank.out

│&nbsp;&nbsp; └── stopwords.txt

Your <sub>index</sub> and <sub>index/api</sub> directories need to be python packages.

<h2>PageRank integration</h2>
In lecture, you learned about PageRank, an algorithm used to determine the relative importance of a website based on the sites that link to that site, and the links to other sites that appear on that website. Sites that are more important will have a higher PageRank score, so they should be returned closer to the top of the search results.

In this project, you are given a set of pages and their PageRank scores in <sub>pagerank.out </sub>, so you do not need to implement PageRank. However, it is still important to understand how the PageRank algorithm works!

Your search engine will rank documents based on both the query-dependent tf-idf score, as well as the query-independent PageRank score. The formula for the score of a query q on a single document d should be:

where <strong>w</strong> is a decimal between 0 and 1, inclusive. The value <strong>w</strong> will be a URL parameter. The <strong>w </strong>parameter represents how much weight we want to give the document’s PageRank versus its cosine similarity with the query. This is a completely different variable from the “w<sub>ik</sub>” given by the formula in Inverted Index with MapReduce. The final score contains two parts, one from pagerank and the other from a tf-idf based cosine similarity score. The <strong>PageRank(d)</strong> is the pagerank score of document <strong>d</strong>, and the <strong>tfIdf(q, d)</strong> is the cosine similarity between the query and the document tf-idf weight vectors. Each weight in a tf-idf weight vector is calculated via the formula in Inverted Index with MapReduce for “w<sub>ik</sub>”. Treat query <strong>q</strong> as a simple AND, non-phrase query(that is, assume the words in a query do not have to appear consecutively and insequence).

Integrating PageRank scores will require creating a second index, which maps each <sub>doc_id</sub> to its corresponding precomputed PageRank score, which is given to you in <sub>pagerank.out </sub>. You can do this where you read the inverted index. This index should be accessed at query time by your index server.

If you still have some confusion with these calculations, please refer to Appendix A

<h2>Returning hits</h2>
When the Index server is run, it will load the inverted index file, pagerank file, and stopwords file into memory and wait for queries. <strong>It should only load the inverted index and pagerank into memory once, when the index server is first started.</strong>

<strong>&nbsp;Note</strong>: The t2 micro instance used to create the AWS instance has a small memory capacity, so please make sure the data structure used to store the inverted index is memory effiicent where possible. You can check how much memory your server is using by starting up the index server and checking the memory footprint of it using top or other MacOS/Windows memory analysis tools.

Every time you send an appropriate request to the index server, it will process the user’s query and use the inverted index loaded into memory to return a list of all of the “hit” <sub>doc_ids </sub>. A hit will be a document that is similar to the user’s query. When finding similar documents, only include documents that have every word from the query in the document. The index server should not load the inverted index or pagerank into memory every time it receives a query!

<h2>Index Server Endpoint</h2>
Route: http://{host}:{port}?w=&lt;w&gt;&amp;q=&lt;query&gt;

Your index server should only have one endpoint, which receives the pagerank weight and query as URL parameters <strong>w</strong> and <strong>q</strong>, and returns the search results, including the relevance score for each result (calculated according to the previous section). For example, the endpoint <sub>?</sub>

w=0.3&amp;q=michigan%20wolverine would correspond to a pagerank weight of 0.3, and a query “michigan wolverine”.

Your index server should return a JSON object in the following format. A full walkthrough of the example is shown in Appendix A.

{

<strong>“hits”</strong>: [

{

<strong>“docid”</strong>: 868657,

<strong>“score”</strong>: 0.071872572435374

}

]

}

The documents in the hits array must be sorted in order of relevance score, with the most relevant documents at the beginning, and the least relevant documents at the end. If multiple documents have the same relevance score, sort them in order of <sub>doc_id</sub> (with the smallest

doc_id first).

When you get a user’s query make sure you remove all stopwords. Since we removed them from our inverted index, we need to remove them from the query. Also clean the user’s query of any nonalphanumeric characters as you did with the inverted index.

<h2>Running the index server</h2>
Install you index server app by running the command below in your project root directory:

$ pip install -e index

To run the index server, you will use environment variables to put the development server in debug mode, specify the name of your app’s python module and locate an additional config file. (These commands assume you are using the bash shell.)

$ export FLASK_DEBUG<strong>=</strong>True

$ export FLASK_APP<strong>=</strong>index

$ export INDEX_SETTINGS<strong>=</strong>config.py

$ flask run –host 0.0.0.0 –port 8001

<ul>
<li>Serving Flask app “index”</li>
<li>Forcing debug mode on</li>
<li>Running on http://127.0.0.1:8001/ (Press CTRL+C to quit)</li>
</ul>
<h2>Common problems</h2>
Make sure that your index server reads stopwords.txt , pagerank.out from the index/index/ directory.

<strong>Pro-tip:</strong> use an absolute path and Python’s <sub>__file__</sub> variable. The following code will result in stopwords_filename = “index/index/stopwords.txt” .

“””index/index/api/views.py”””

index_package_dir <strong>=</strong> os<strong>.</strong>path<strong>.</strong>dirname(os<strong>.</strong>path<strong>.</strong>dirname(__file__)) stopwords_filename <strong>=</strong> os<strong>.</strong>path<strong>.</strong>join(index_package_dir, “stopwords.txt”)

<h2>Testing</h2>
Once you have implemented your Index Server, you should be able to pass all tests in test_index_server_public.py .

$ pytest -v tests/test_index_server_public.py

<h1>Search interface</h1>
The third component of the project is a React driven interface for the search engine. The search interface app will provide a GUI for the user to enter a query and specify a Pagerank weight, and will then send a request to your index server. When it receives the search results from the index server, it will display them on the webpage.

<h2>Directory structure</h2>
As mentioned earlier, in this project since you have two separate servers, the index server and the search server, you will need a separate directory for you search server. Your search interface server code is going to be inside the directory <sub>search/search</sub> and your <sub>setup.py</sub> is going to be inside the directory <sub>search </sub>. Your search server is supposed to be a python package. Below is an example of what your final search directory structure should look like.

$ tree search

├── search

│&nbsp;&nbsp; ├── package.json

│&nbsp;&nbsp; ├── package-lock.json

│&nbsp;&nbsp; ├── node_modules

│&nbsp;&nbsp; │&nbsp;&nbsp; └── */

│&nbsp;&nbsp; ├── search

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── api

│&nbsp;&nbsp; │&nbsp;&nbsp; │&nbsp;&nbsp; └── *.py

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── js

│&nbsp;&nbsp; │&nbsp;&nbsp; │&nbsp;&nbsp; └── *.jsx

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── config.py

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── sql

│&nbsp;&nbsp; │&nbsp;&nbsp; │&nbsp;&nbsp; └── wikipedia.sql

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── static

│&nbsp;&nbsp; │&nbsp;&nbsp; │&nbsp;&nbsp; └── js

│&nbsp;&nbsp; │&nbsp;&nbsp; │&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; └── bundle.js

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── templates

│&nbsp;&nbsp; │&nbsp;&nbsp; │&nbsp;&nbsp; └── *.html

│&nbsp;&nbsp; │&nbsp;&nbsp; ├── var

│&nbsp;&nbsp; │&nbsp;&nbsp; │&nbsp;&nbsp; └── wikipedia.sqlite3

│&nbsp;&nbsp; │&nbsp;&nbsp; └── views

│&nbsp;&nbsp; │&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; └── *.py

│&nbsp;&nbsp; ├── setup.py

│&nbsp;&nbsp; └── webpack.config.js

Your <sub>search </sub>, <sub>views </sub>, and <sub>api</sub> directories need to be Python packages.

<h2>Database</h2>
You will need to create a new database for project 5, with a table called Documents as follows:

docid : INT and PRIMARY KEY title : <sub>VARCHAR</sub> with max length 100 categories : VARCHAR with max length 5000 image : <sub>VARCHAR</sub> with max length 200 summary : <sub>VARCHAR</sub> with max length 5000

The SQL to create this table and load the necessary data into it is provided in search/search/sql/wikipedia.sql inside the starter files.

<h2>GUI</h2>
Make a simple search interface for your database of Wikipedia articles which allows users to input a <strong>query</strong> and a <strong>w</strong> value, and view a ranked list of relevant docs. This is the main route ( http://{host}:{port}/ ).

Users can enter their <strong>query</strong> into a text input box ( <sub>&lt;input type=”text”&gt; </sub>), and specify the <strong>w</strong> value using a slider. The query is executed when a user presses a ( <sub>&lt;input type=”submit”&gt; </sub>). You can assume anyone can use your search engine; you do not need to worry about access rights or sessions like past projects. Your engine should receive a simple AND, non-phrase query (that is, assume the words in a query do not have to appear consecutively and in-sequence), and return the ranked list of docs. Your search results will be titles of Wikipedia documents, displayed exactly as they appear in the database. Search results will show <strong>at most 10 documents</strong>. Any other content should appear below.

This page must include a slider ( <sub>&lt;input type=”range”&gt; </sub>) that will set the <strong>w</strong> GET query parameter in the URL, and will be a decimal value between 0-1, inclusive. You should set the range slider’s step value to be 0.01.

When the user clicks the submit button of the search GUI, you should fetch the appropriate titles from the index server. For each title returned, display the title in a p tag with a class=”doc_title” ( <sub>&lt;p className=”doc_title”&gt; </sub>) as well as a button to display the summary for that title with a value=”Show Summary”( &lt;input type=”submit” value=”Show Summary”&gt; )

If there are no search results, no action is required

Upon clicking the ‘show summary’ button for a title, the list of results sould be <em>replaced</em> with a summary of the document. You may simply place the summary data within a <sub>&lt;p&gt;</sub> tag with a

class=”doc\_summary” ( &lt;p className=”doc_summary”&gt; ). In addition to having this summary, this

page will also have a “Similar Documents” section, which will show <strong>at most 10 documents</strong> using w=0.15, and the current document’s title as the search query. For each related document title, render a p tag with class=”doc_title” ( &lt;p className=”doc_title”&gt; ).

<h2>Running the search server</h2>
Install you search server app by running the command below in your project root directory:

$ pip install -e search

To run the search server, you will use environment variables to put the development server in debug mode, specify the name of your app’s python module and locate an additional config file. (These commands assume you are using the bash shell.)

$ export FLASK_DEBUG<strong>=</strong>True $ export FLASK_APP<strong>=</strong>search

$ export SEARCH_SETTINGS<strong>=</strong>config.py

$ flask run –host 0.0.0.0 –port 8000

<ul>
<li>Serving Flask app “search”</li>
<li>Forcing debug mode on</li>
<li>Running on http://127.0.0.1:8000/ (Press CTRL+C to quit)</li>
</ul>
In order, to be able to search on the search server, you must have your index server up and running, since it is the response of the index server that the search server uses to display the search results.

<h2>Shell scripts to launch both servers</h2>
You will be responsible for writing shell scripts to launch both the index server and the search server. Hint: these will be somewhat similar to last project’s bin/mapreduce script. The name of these scripts must be bin/index and bin/search .

Example: start search.

$ ./bin/search start starting search server …

+ export FLASK_APP=search

+ export SEARCH_SETTINGS=config.py

+ flask run –host 0.0.0.0 –port 8000 &amp;&gt; /dev/null &amp;

Example: stop search.

$ ./bin/search stop stopping search server …

+ pkill -f ‘flask run –host 0.0.0.0 –port 8000’ Example: restart search. Your PIDs may be different.

$ ./bin/search restart stopping search server …

+ pkill -f ‘flask run –host 0.0.0.0 –port 8000’ starting search server …

+ export FLASK_APP=search

+ export SEARCH_SETTINGS=config.py

+ flask run –host 0.0.0.0 –port 8000 &amp;&gt; /dev/null &amp;

Example: start search when something is already running on port 8000

$ ./bin/search start

Error: a process is already using port 8000 Example: start index.

$ ./bin/index start starting index server …

+ export FLASK_APP=index

+ flask run –host 0.0.0.0 –port 8001 &amp;&gt; /dev/null &amp; Example: stop index.

$ ./bin/index stop stopping index server …

+ pkill -f ‘flask run –host 0.0.0.0 –port 8001’ Example: restart index.

$ ./bin/index restart stopping index server …

+ pkill -f ‘flask run –host 0.0.0.0 –port 8001’ starting index server …

+ export FLASK_APP=index

+ flask run –host 0.0.0.0 –port 8001 &amp;&gt; /dev/null &amp;

Example: start index when something is already running on port 8001

$ ./bin/index start

Error: a process is already using port 8001

flask run –host 0.0.0.0 –port 8000 &amp;&gt; /dev/null &amp; will start up your flask server in the

background. The <sub>&amp;&gt; /dev/null</sub> will prevent your Flask app from outputting text to the terminal.

<h2>Index database management script</h2>
You will also write a database script for the index server.

Example create.

$ ./bin/indexdb create

+ mkdir -p search/search/var/

+ sqlite3 search/search/var/wikipedia.sqlite3 &lt; search/search/sql/wikipedia.sql Example create when database already exists.

$ ./bin/indexdb create

Error: database already exists Example destroy.

$ ./bin/indexdb destroy

+ rm -f search/search/var/wikipedia.sqlite3 Example reset.

$ ./bin/indexdb reset

+ rm -f search/search/var/wikipedia.sqlite3

+ mkdir -p search/search/var/

+ sqlite3 search/search/var/wikipedia.sqlite3 &lt; search/search/sql/wikipedia.sql

<h2>Deploy to AWS</h2>
<a href="https://eecs485staff.github.io/p2-insta485-serverside/setup_aws.html#deploy-a-web-app">You should have already created an AWS account and instance (</a><a href="https://eecs485staff.github.io/p2-insta485-serverside/setup_aws.html#deploy-a-web-app">instructions</a><a href="https://eecs485staff.github.io/p2-insta485-serverside/setup_aws.html#deploy-a-web-app">). </a><a href="https://eecs485staff.github.io/p2-insta485-serverside/setup_aws.html#deploy-a-web-app">Resume the </a><a href="https://eecs485staff.github.io/p2-insta485-serverside/setup_aws.html#deploy-a-web-app">AWS Tutorial – Deploy a web app</a><a href="https://eecs485staff.github.io/p2-insta485-serverside/setup_aws.html#deploy-a-web-app">.</a>

Once you have installed your front-end, go to your instance. In the “Description”, click on the name of your security group.

In this case, the security group is “launch-wizard 2”.

On this page, click on “Actions”, then “Edit inbound rules”.

<table>
<tbody>
<tr>
<td width="55"></td>
</tr>
<tr>
<td></td>
<td></td>
</tr>
</tbody>
</table>
Then, add a “Custom TCP Protocol” for port 8001.

Remember that you need to run two servers, the index server and search server.

$ gunicorn -b localhost:8000 -D search:app

$ gunicorn -b 0.0.0.0:8001 -D index:app

After you have deployed your site, download the search page along with a log. Also download the index server’s response with a log. Do this from your local machine.

$ pwd

/Users/awdeorio/src/eecs485/p5-search-engine

$ curl -v &lt;Public DNS <strong>(</strong>IPv4<strong>)&gt;</strong>/ <strong>&gt;</strong> deployed_search.html 2&gt; deployed_search.log

$ curl -v “&lt;Public DNS (IPv4)&gt;:8001/?q=world%20flags&amp;w=0.5” <strong>&gt;</strong> deployed_index.json 2&gt; deplo

Verify that the output in deployed_search.log and deployed_index.log doesn’t include errors like “Couldn’t connect to server”.

<h1>Testing</h1>
Run published unit tests.

$ pwd

/Users/awdeorio/src/eecs485/p5-search-engine $ pytest -v

<h2>Code style</h2>
As in previous projects, all your Python code for the Flask servers is expected to be <sub>pycodestyle </sub>, pydocstyle , and <sub>pylint</sub> compliant. You don’t need to lint the mapper/reducer executables

(although it may be a good idea to do so still!)

Also as usual, you may not use any external dependencies aside from what is provided in the setup.py’s.

<h1>Submitting and grading</h1>
One team member should register your group on the autograder using the <em>create new invitation </em>feature.

Submit a tarball to the autograder, which is linked from <a href="https://eecs485.org/">https://eecs485.org</a><a href="https://eecs485.org/">.</a> Include the <sub>–</sub>disable-copyfile flag only on macOS.

$ tar \

-cjvf submit.tar.bz2 \

–disable-copyfile \

–exclude ‘*input.txt’ \

–exclude ‘*/input/*’ \

–exclude ‘*/input_multi/*’ \

–exclude ‘*output*’ \

–exclude ‘*__pycache__*’ \

–exclude ‘*node_modules*’ \

–exclude ‘*stopwords.txt’ \

–exclude ‘*.out’ \

–exclude ‘*.sql’ \

–exclude ‘*.sqlite3’ \

–exclude ‘*.jar’ \

–exclude ‘*.egg-info’ \

–exclude ‘*var*’ \

–exclude ‘*tmp*’ \

–exclude ‘hadoop/inverted_index/inverted_index.txt’ \&nbsp;&nbsp; bin \&nbsp;&nbsp; hadoop \ &nbsp;&nbsp;hadoop/inverted_index/input_split.py \&nbsp;&nbsp; index \&nbsp;&nbsp; search \&nbsp;&nbsp; deployed_index.json \&nbsp;&nbsp; deployed_index.log \&nbsp;&nbsp; deployed_search.html \&nbsp;&nbsp; deployed_search.log

Note that the submission command uses the <sub>-j</sub> flag: This tells <sub>tar</sub> to use the <sub>bzip2 </sub>compression algorithm. <sub>bzip2</sub> is slower than <sub>gzip</sub> (which we used in past projects), but generally results in better compression and smaller file sizes. <strong>Make sure your submission tarball is around 10MB.</strong>

$ du -h submit.tar.bz2

9.6M &nbsp;&nbsp; submit.tar.gz

<h2>Rubric</h2>
This is an approximate rubric.

<table width="372">
<tbody>
<tr>
<td width="305"><strong>Deliverable</strong></td>
<td width="67"><strong>Value</strong></td>
</tr>
<tr>
<td width="305">Public tests</td>
<td width="67">50%</td>
</tr>
<tr>
<td width="305">Hidden unit tests run after the deadline</td>
<td width="67">40%</td>
</tr>
<tr>
<td width="305">Public style tests</td>
<td width="67">10%</td>
</tr>
</tbody>
</table>
<h1>FAQ</h1>
<h2>API Request URLs</h2>
When you are attempting to send a request to <strong>search interface API</strong> from your <strong>ReactJS search interface frontend</strong>, do not include the <sub>host:port</sub> in the url you are attempting to fetch.

If you want to send a request to your <strong>index server API</strong> from your <strong>search interface API</strong>, you will want to include the following <sub>host:port</sub> pair in the url you are attempting to send a request to: http://localhost:8001

<h1>Appendix A: TFIDF Calculation Walkthrough</h1>
You have a query, let’s make a query vector for that

You have a document, let’s make a document vector for that

Let’s define a norm factor for our document

Let’s define a norm factor for our query

Note: that the IDFs for both norm factors come from the inverted index. The norm factor for the document can be lifted from your inverted index (but you have sqrt it), where as the query norm factor needs to be computed on the fly.

If you have defined your query and document vectors this way, then the final score will be

<h2>Example</h2>
Let’s walk through an example for the query <sub>?w=0.3&amp;q=michigan%20wolverine </sub>. The query is michigan wolverine . The weight of PageRank is <sub>0.3</sub> and the weight tf-idf is <sub>0.7 </sub>.

<h3>Read inverted index and PageRank</h3>
Search the inverted index for <sub>michigan </sub>.

$ egrep ‘^michigan[[:space:]]’ ./index/index/inverted_index.txt michigan &nbsp;&nbsp;&nbsp;&nbsp; 1.509960674077735 10883747 14 8852.693606436345 … $ egrep ‘^wolverine[[:space:]]’ ./index/index/inverted_index.txt wolverine &nbsp;&nbsp;&nbsp;&nbsp; 2.669184007846121 5791422 1 66539.45074152622 …

We see that the idf for <sub>michigan</sub> is <sub>1.509</sub> and the idf for <sub>wolverine</sub> is <sub>2.669 </sub>. When we look at the docids for <sub>michigan</sub> and <sub>wolvinere </sub>, we see that there is one document (docid <sub>868657 </sub>) that contains both terms.

$ egrep ‘^(michigan|wolverine)[[:space:]]’ ./index/index/inverted_index.txt | grep 868657 wolverine … 868657 1 126536.87039603827 … michigan … 868657 46 126536.87039603827 …

In document 868657 , michigan appears 46 times, and wolverine occurs 1 time.

We’ll also read the value of PageRank for document <sub>868657</sub> from <sub>pagerank.out </sub>.

$ egrep 868657 ./index/index/pagerank.out

868657,5.41822e-06

<h3>Query vector and document vector</h3>
The Query vector has one position for each term ( <sub>[“michigan”, “wolverine”] </sub>). Each position is a number calculated as &lt;term frequency in query&gt; * &lt;idf&gt; .

q = [1*1.509, 1*2.669]&nbsp;&nbsp; = [1.509, 2.669]

The Document vector similarly has one position for each term ( <sub>[“michigan”, “wolverine”] </sub>). Each position is a number calculated as &lt;term frequency in document&gt; * idf .

d = [46*1.509, 1*2.669]

= [69.458, 2.669] <strong>tf-idf</strong>

Compute the dot product of <sub>q</sub> and <sub>d </sub>. q * d = 112.003

Compute the normalization factor for the query. The normalization factor is the length of the query vector, which is the sum-of-squares of the query vector.

q = [1.509, 2.669] norm_q = sqrt(1.509^2 + 2.669^2) = 3.066

Compute the normalization factor for the document, which is the square root of the normalization factor read from the inverted Index.

norm_d_squared = 126536.870 norm_d = sqrt(126536.870)

= 355.7128124 Compute tf-idf.

tfidf = q * d / (norm_q * norm_d)

= 112.003 / (3.066 * 355.712)

= 0.102

<h3>Weighted score</h3>
Finally, we combine tf-idf and PageRank using the weight.

weighted_score = w * PageRank + (1-w) (tdidf)

= (0.3 * 5.418e-06) + (1-0.3) * (0.102)

= 0.071

<h1>Appendix B: Installing Real Hadoop</h1>
Although not needed for this project, below are the steps to install hadoop on OSX and WSL if you want to play around with it.

If you are on OSX, install Hadoop with Homebrew

$ brew cask install java

$ brew install hadoop

If you are on Ubuntu Linux, Ubuntu Linux VM or Windows 10 WSL, you will have to install Hadoop manually. <strong>OSX users skip the following. Resume below, where specified </strong>Install Java

$ sudo -s&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <em># Become root</em>

$ sudo apt-get update

$ sudo apt-get install default-jdk&nbsp;&nbsp; <em># Install Java </em>$ java -version&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <em># Check Java version </em>openjdk version “1.8.0_151”

OpenJDK Runtime Environment (build 1.8.0_151-8u151-b12-0ubuntu0.16.04.2-b12)

OpenJDK 64-Bit Server VM (build 25.151-b12, mixed mode)

Download Hadoop and unpack.

$ cd /opt

$ wget http://apache.osuosl.org/hadoop/common/hadoop-2.8.5/hadoop-2.8.5.tar.gz

$ wget https://dist.apache.org/repos/dist/release/hadoop/common/hadoop-2.8.5/hadoop-2.8.5.

$ shasum -a 256 hadoop-2.8.5.tar.gz e8bf9a53337b1dca3b152b0a5b5e277dc734e76520543e525c301a050bb27eae&nbsp; hadoop-2.8.5.tar.gz

$ grep SHA256 hadoop-2.8.5.tar.gz.mds

SHA256 = E8BF9A53 337B1DCA 3B152B0A 5B5E277D C734E765 20543E52 5C301A05 0BB27EAE

$ tar -xvzf hadoop-2.8.5.tar.gz

$ rm hadoop-2.8.5.tar.gz hadoop-2.8.5.tar.gz.mds

Locate the path to your Java interpreter.

$ which java | xargs readlink -f | sed ‘s:bin/java::’

/usr/lib/jvm/java-8-openjdk-amd64/jre/

Edit /opt/hadoop-2.8.5/etc/hadoop/hadoop-env.sh to change the JAVA_HOME .

<em>#export JAVA_HOME=${JAVA_HOME}&nbsp; # remove/comment </em>export JAVA_HOME<strong>=</strong>/usr/lib/jvm/java-8-openjdk-amd64/jre

Write a launch script, /usr/local/bin/hadoop

<em>#!/bin/bash</em>

exec “/opt/hadoop-2.8.5/bin/hadoop” “$@”

Make the script executable and check that it’s working.

$ chmod +x /usr/local/bin/hadoop

$ which hadoop

/usr/local/bin/hadoop

$ hadoop&nbsp; -h

Usage: hadoop [–config confdir] [COMMAND | CLASSNAME]

<em>… </em>

$ exit&nbsp; <em># drop root privileges</em>

<h2>OSX Java Home Error</h2>
<strong>Note to OSX users:</strong> If you run Hadoop and Hadoop is unable to find JAVA_HOME, please refer to the fix below.

<ol>
<li>Find <sub>hadoop-env.sh </sub>. You location might be different.</li>
</ol>
$ find / -name hadoop-env.sh

/usr/local/Cellar/hadoop/2.8.1/libexec/etc/hadoop/hadoop-env.sh

<ol start="2">
<li>Uncomment and edit the export JAVA_HOME line in hadoop-env.sh :</li>
</ol>
<em># The java implementation to use.</em>

export JAVA_HOME<strong>=</strong>“$(/usr/libexec/java_home)”
