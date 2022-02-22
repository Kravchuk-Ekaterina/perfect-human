# Perfect human project
## 1. Converting the raw 23andMe data to vcf
I use plink - tool widely used in population genetics https://www.cog-genomics.org/plink/ <br>
I remove all SNPs corresponding to deletions and insertions, to make the file compatible with annotation tools<br>
The command is:<br>
```bash
~/Libs/plink_1_09/plink --23file <23_and_me_input.txt> --recode vcf --out snps_clean --output-chr MT --snps-only just-acgt
```
In my case:
```bash
home/kate_the_snail/Загрузки/plink_linux_x86_64_20210606/plink --23file ./data/SNP_raw_v4_Full_20170514175358.txt --recode vcf --out snps_clean --output-chr MT --snps-only just-acgt
```

