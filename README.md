# q2-comp

QIIME2 plugin for comparison of results <br>
For descriptions on how to install and run this plugin, see  <a href="https://github.com/dianahaider/q2-comp/wiki">here</a>.

## Getting started

For all vis has the option to change palette, style and context of visualizations.

### Alpha

This function xyz

```
qiime comp alpha-frequency \
  --i-tables table1.qza table2.qza table3.qza \
  --m-metadata METADATA.txt \
  --p-metadata-col depth \
  --o-visualization visualization_frequency.qzv
```
<a href="https://github.com/dianahaider/q2-comp/wiki">visualization_frequency.qzv</a>

Can also abc

```
qiime comp alpha-index \
  --i-alpha-diversity-index shannon1.qza shannon2.qza shannon3.qza \
  --m-metadata METADATA.txt \
  --p-metadata-col depth \
  --o-visualization visualization_index.qzv
```
<a href="https://github.com/dianahaider/q2-comp/wiki">visualization_index.qzv</a>

And just def

```
qiime comp alpha-core \
  --i-tables table1.qza table2.qza table3.qza \
  --i-alpha-diversity shannon1.qza shannon2.qza shannon3.qza \
  --m-metadata METADATA.txt \
  --p-metadata-col depth \
  --o-visualization visualization_index.qzv
  --o-visualization visualization_frequency.qzv
  --o-visualization visualization_merged.qzv

```
<a href="https://github.com/dianahaider/q2-comp/wiki">visualization_index.qzv</a>
<a href="https://github.com/dianahaider/q2-comp/wiki">visualization_frequency.qzv</a>
<a href="https://github.com/dianahaider/q2-comp/wiki">visualization_merged.qzv</a>

### Denoise

This functions xyz

```
qiime comp denoise \
  --i-stats stats1.qza stats.qza stats.qza \
  --p-labels Method1 Method2 Method3
  --o-visualization visualization.qzv
```
<a href="https://github.com/dianahaider/q2-comp/wiki">visualization.qzv</a>
