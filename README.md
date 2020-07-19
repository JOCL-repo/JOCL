# JOCL

The project JOCL consists of two parts: (1) GraphConstruction; (2) LearnAndInference.

1. Unzip the files FreebaseEntityInWiki2.part01 (02, 03, 04).rar and combine them as a file named FreebaseEntityInWiki2. Put the file FreebaseEntityInWiki2 in the folder "GraphConstruction\intermedia_data".
2. Unzip all the files of the folder "GraphConstruction\intermedia_data".
3. Unzip the files original_data.rar and external_data.rar and put them in the folder "GraphConstruction".
4. Download crawl-300d-2M.vec (https://fasttext.cc/docs/en/english-vectors.html) and put it in the folder "GraphConstruction".
5. Run the file GraphConstruction\GraphGen.py to construct the factor graph model of the framework JOCL.
6. Run the file LearnAndInference\JOCL.cpp to learn parameters of JOCL and inference.
7. Run the file GraphConstruction\Evaluation\Final-Evaluation.py to test the performance of JOCL. 

We store some intermediate data files generated by each step in the corresponding position.  
If you want to obtain the results of JOCL quickly, please start step 4 derectly.


Experiments:

1. All the results of the baselines for NP canonicalization are taken from SIST[1].
2. We randomly sample 35 non-singleton RP groups and manually label them as the ground truth for RP canonicalization like SIST. 
   We present labeled RP groups in the folder "Experiments\RP canonicalization". 
   All the results of the baselines for RP canonicalization are taken from SIST.
3. We present some results of baselines (i.e., Earl, Falcon, Spotlight, Tagme) for OKB entity linking in the folder "Experiments\OKB entity linking".
4. We randomly sample 100 OIE triples and manually label each RP as the ground truth for OKB relation linking. 
   We present labeled OIE triples and some results of baselines （i.e., Rematch, Earl, Falcon） for OKB relation linking in the folder "Experiments\OKB relation linking".
 
 
[1] Canonicalization of open knowledge bases with side information from the source text. ICDE, 2019, 950-961.
 

 
