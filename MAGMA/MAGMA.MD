<h2> 相关资源的下载网址<br>
<h4>https://cncr.nl/research/magma/<br>
<h2>步骤<br>
<h2>magma三步骤<br>
<h4>注释：将自己的SNP根据染色体位置注释到基因上<br>
<h4>magma \
    --annotate \
    --snp-loc [SNPLOC_FILE] \
    --gene-loc [GENELOC_FILE] \
    --out [ANNOT_PREFIX] <br>
<h4>Gene-based 分析<br>
<h4>magma \
    --bfile [REFDATA] \
    --pval [PVAL_FILE] \
    N=[N] \
    --gene-annot [ANNOT_PREFIX].genes.annot \
    --out [GENE_PREFIX]<br>
<h4>基因集/通路分析<br>
<h4>magma \
    --gene-results [GENE_PREFIX].genes.raw \
    --set-annot [SET_FILE] \
    --out [GS_PREFIX]<br>
