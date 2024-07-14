<h2>Step 0: Munge features<br>
<h4>python munge_feature_directory.py \
 --gene_annot_path example/data/utils/gene_annot_jun10.txt \
 --feature_dir example/data/features_raw/ \
 --save_prefix example/data/features_munged/pops_features \
 --max_cols 500 <br>
 <h2>Step 1: Generate MAGMA scores<br>
 <h4>./magma \
 --bfile {PATH_TO_REFERENCE_PANEL_PLINK} \
 --gene-annot {PATH_TO_MAGMA_ANNOT}.genes.annot \
 --pval {PATH_TO_SUMSTATS}.sumstats ncol=N \
 --gene-model snp-wise=mean \
 --out {OUTPUT_PREFIX} <br>
 <h2>Step 2: Run PoPS<br>
 <h4>python pops.py \
 --gene_annot_path example/data/utils/gene_annot_jun10.txt \
 --feature_mat_prefix example/data/features_munged/pops_features \
 --num_feature_chunks 2 \
 --magma_prefix example/data/magma_scores/PASS_Schizophrenia \
 --control_features_path example/data/utils/features_jul17_control.txt \
 --out_prefix example/out/PASS_Schizophrenia<br>
 
 
