# WGBS data analysis
## Marsden project - Objective 1:
## Wild fish sampled along the NZ coasts

Author: Dafni Anastasiadi  
Date: March 2023

Samples were pooled per area (11 pools). WBGS libraries were prepared and sequenced by Novogene. Details of the library prep protocol can be found here:  
file://///storage.powerplant.pfr.co.nz/workspace/cfndxa/MarsdenObj1/Sequencing_WBGS/X201SC20071998-Z01-F001/02.Report_X201SC20071998-Z01-F001/X201SC20071998-Z01-F001_Report.html


```bash
ls
```


```bash
module avail
```

    ---------------- [1;94m/software/EnvironmentModules/4.7.1/modulefiles[0m ----------------
    dot  module-git  module-info  modules  null  use.own  
    
    ------------------- [1;94m/software/powerPlant/modulefiles/custom[0m --------------------
    1SynChro/1.15                                         vcflib/1.0.2            
    3d-dna/180922                                         vcflib/50a3229          
    A5-miseq/20160825                                     vcflib/73b7f13          
    abyss/2.0.2                                           vcflib/586c5ae          
    abyss/2.2.4                                           vcftools/0.1.12         
    adapterremoval/2.2.2                                  vcftools/0.1.14         
    AfterQC/0.9.1                                         velvet/1.2.10           
    AfterQC/0.9.5                                         VersioningService/69    
    allpathslg/44837                                      VersioningService/91    
    allpathslg/44913                                      VersioningService/92    
    allpathslg/49722                                      VersioningService/93    
    allpathslg/50191                                      VersioningService/103   
    allpathslg/52488                                      VersioningService/104   
    amos/3.1.0                                            vg/1.7.0                
    angsd-wrapper/7224db2                                 vg/1.8.0                
    angsd/0.913                                           vg/1.9.0                
    angsd/0.917                                           vg/1.10.0               
    angsd/0.917-116-g5d087b2                              vg/1.11.0               
    angsd/0.918                                           vg/1.12.0               
    angsd/0.919                                           vg/1.12.1               
    angsd/0.921                                           vg/1.13.0               
    angsd/0.922                                           ViennaRNA/2.2.2         
    angsd/0.923                                           VISOR/1.1               
    angsd/0.925                                           vsearch/2.3.2           
    angsd/0.937                                           wgs/8.3rc2              
    anytag/2.5.2                                          whatshap/0.14.1-py36_0  
    apptainer/1.1                                         winnowmap/2.0.0         
    apsim/7.9-r4047                                       wise/2.4.1              
    apsim/7.10-r49ace54f9c8a670190aef9d8d0fb9d5477bb1534  wkhtmlox/0.12.3         
    apsimx/2018.01.30.2253                                wtdbg2/2.2              
    apsimx/2018.09.28.3099                                
    apsimx/2019.01.08.3392                                
    apsimx/2019.04.03.3693                                
    apsimx/2019.06.05.3920                                
    apsimx/2019.07.18.4025                                
    apsimx/2019.10.04.4236                                
    apsimx/2020.04.09.5012                                
    apsimx/2020.08.04.5350                                
    apsimx/2020.10.21.5755                                
    apsimx/2020.11.27.5887                                
    apsimx/2021.04.15.6139                                
    apsimx/2021.9.21.6799                                 
    apsimx/2021.10.8.6835                                 
    apsimx/2022.04.7021.0                                 
    apsimx/2022.06.7046.0                                 
    apsimx/2022.09.7085.0                                 
    arcs/1.0.6                                            
    art/MountRainier                                      
    aspera-cli/3.7.2.354.010c3b8                          
    assemblathon_stats/14dfdab                            
    assemblathon_stats/2011_10_13                         
    asub/2.1                                              
    asub/2.2                                              
    augustus/3.2.2                                        
    augustus/3.3                                          
    augustus/3.3.1                                        
    augustus/3.3.3                                        
    aws-cli/2.0.43                                        
    badread/0.2.0                                         
    bam2fastx/1.3.0                                       
    bambam/1.4                                            
    bamtools/2.3.0                                        
    bamtools/2.4.0                                        
    bats/0.4.0                                            
    BBMap/37.28                                           
    BBMap/37.53                                           
    BBMap/37.93                                           
    BBMap/38.33                                           
    bcftools/1.3.1                                        
    bcftools/1.6                                          
    bcftools/1.9                                          
    bcftools/1.10.2                                       
    bcftools/1.12                                         
    bcftools/1.16                                         
    bcgTree/1.0.8                                         
    beagle/4.0                                            
    beagle/4.1                                            
    BEAST/1.8.4                                           
    BEAST2/2.4.7                                          
    bedops/2.4.39                                         
    bedtools/2.20.1                                       
    bedtools/2.21.0                                       
    bedtools/2.27.1                                       
    bedtools/2.30.0                                       
    bfc-submitted/v1                                      
    biobakery_workflows/v3.0.0-alpha.7                    
    biobambam/0.0.191                                     
    biobambam2/2.0.44                                     
    biobambam2/2.0.106                                    
    bismark/0.19.1                                        
    bismark/0.20.0                                        
    bismark/0.23.0                                        
    blasr/5.2.badc092                                     
    blast/2.2.26                                          
    BLAT/36                                               
    blobtools/1.0                                         
    bonito/0.3.6                                          
    bonito/0.4.0                                          
    boost/1_61_0                                          
    boost/1_61_0-dev                                      
    boost/1_65_1                                          
    boost/1_65_1-dev                                      
    bowtie/1.0.0                                          
    bowtie2/2.2.5                                         
    bowtie2/2.2.9                                         
    bowtie2/2.3.4.3                                       
    BRAKER/1.9                                            
    BRAKER/1.11                                           
    BRAKER/2.0.1                                          
    BRAKER/2.0.4                                          
    BRAKER/2.0.5                                          
    BRAKER/2.1.0                                          
    BRAKER/2.1.2                                          
    BRAKER/2.1.5                                          
    breakdancer/4e44b43                                   
    BSseeker2/2.1.5                                       
    BUSCO/v1.2                                            
    BUSCO/v2.0                                            
    BUSCO/v3.0.2                                          
    BUSCO/v4.1.2                                          
    BUSCO/v4.1.4                                          
    BUSCO/v5.1.2                                          
    BUSCO/v5.2.2                                          
    bwa/0.7.12                                            
    bwa/0.7.15                                            
    bwa/0.7.17                                            
    cafe/5.0.0                                            
    canu/1.3                                              
    canu/1.5                                              
    canu/1.6                                              
    canu/1.7                                              
    canu/2.1.1                                            
    cd-hit/4.6.1                                          
    cdo/1.7.0                                             
    cdo/1.9.3                                             
    cdo/1.9.5                                             
    cegma/v2.4.010312                                     
    cegma/v2.5                                            
    checkm/1.0.6                                          
    checkm/1.0.7                                          
    checkm/1.0.8                                          
    checkm/1.0.10                                         
    checkm/1.0.11                                         
    checkm/1.0.12                                         
    checkm/1.0.13                                         
    checkm/1.1.3                                          
    chromonomer/1.07                                      
    chromosomer/0.1.3                                     
    clust/1.12.0                                          
    clustal-omega/1.2.4                                   
    cndsrc/2010.10.11                                     
    cndsrc/2017.11.30                                     
    cnvnator/0.3.3                                        
    cnvnator/0.4.1                                        
    CodingQuarry/2.0                                      
    COGNATE/v1.0                                          
    colordiff/1.0.18                                      
    conda/4.5.1                                           
    conda/4.8.2                                           
    conda/4.10.3                                          
    conda/22.9.0                                          
    conda/23.1.0                                          
    cookiecutter/1.0.0                                    
    corset/1.09                                           
    crema/173e9a4                                         
    crisp/c6cd86e                                         
    crossmap/0.3.3                                        
    csvkit/1.0.2                                          
    csvkit/1.0.4                                          
    cufflinks/2.2.1                                       
    cutadapt/1.10                                         
    cutadapt/1.15                                         
    cutesv/1.0.10                                         
    dammit/1.2                                            
    data-registry/1.0                                     
    data-registry/1.0-dev                                 
    data-registry/1.0-test                                
    deepsig/b719cec                                       
    deepvariant/0.7.2-py27h5d9141f_1                      
    deepvariant/1.2.0                                     
    deepvariant/1.4.0                                     
    deepvariant/1.4.0-gpu                                 
    diamond/0.9.24                                        
    Disco/1.1-beta                                        
    docker-compose/1.7.1                                  
    docker-compose/1.11.2                                 
    dtool/3.25.0                                          
    dvc/1.6.1                                             
    dvc/1.11.16                                           
    dvc/2.1.0                                             
    dvc/2.8.1                                             
    dvc/2.8.2                                             
    dvc/2.40.0                                            
    DWGSIM/0561546                                        
    e-PCR/2.3.9                                           
    e-utilities/5.40                                      
    ea-utils/1.1.2-484                                    
    ea-utils/1.1.2-537                                    
    ea-utils/1.1.2-806                                    
    ea-utils/1.04.807                                     
    eddypro-engine/5.1.1                                  
    eddypro-engine/5.2.0                                  
    eddypro-engine/5.2.1                                  
    eddypro-engine/6.0.0                                  
    eddypro-engine/6.1.0                                  
    eddypro-engine/6.2.0                                  
    eddypro-engine/6.2.1                                  
    edta/1.8.3                                            
    edta/1.9.0                                            
    EffectorP/1.0                                         
    eg-all/91                                             
    eg-web-bacteria/91                                    
    eg-web-common/91                                      
    eg-web-fungi/91                                       
    eg-web-metazoa/91                                     
    eg-web-plants/91                                      
    eg-web-protists/91                                    
    eg-web-search/91                                      
    eg-web-testsuite/91                                   
    ehive/2.4                                             
    eigensoft/7.2.1                                       
    eman2/2.3                                             
    emboss/6.4.0                                          
    emboss/6.5.7                                          
    emboss/6.6.0                                          
    emirge/0.61.1                                         
    ensembl-analysis/69                                   
    ensembl-analysis/91                                   
    ensembl-analysis/92                                   
    ensembl-analysis/93                                   
    ensembl-analysis/103                                  
    ensembl-analysis/104                                  
    ensembl-api/69                                        
    ensembl-api/91                                        
    ensembl-api/92                                        
    ensembl-api/93                                        
    ensembl-api/103                                       
    ensembl-api/104                                       
    ensembl-compara/69                                    
    ensembl-compara/91                                    
    ensembl-compara/92                                    
    ensembl-compara/93                                    
    ensembl-compara/103                                   
    ensembl-compara/104                                   
    ensembl-funcgen/69                                    
    ensembl-funcgen/91                                    
    ensembl-funcgen/92                                    
    ensembl-funcgen/93                                    
    ensembl-funcgen/103                                   
    ensembl-funcgen/104                                   
    ensembl-genebuild/69                                  
    ensembl-genebuild/91                                  
    ensembl-genebuild/92                                  
    ensembl-genebuild/93                                  
    ensembl-genebuild/103                                 
    ensembl-genebuild/104                                 
    ensembl-git-tools/d55068a                             
    ensembl-hive-openlava/69                              
    ensembl-hive-openlava/91                              
    ensembl-hive-openlava/92                              
    ensembl-hive-openlava/93                              
    ensembl-hive/69                                       
    ensembl-hive/91                                       
    ensembl-hive/92                                       
    ensembl-hive/93                                       
    ensembl-hive/103                                      
    ensembl-hive/104                                      
    ensembl-io/69                                         
    ensembl-io/91                                         
    ensembl-io/92                                         
    ensembl-io/93                                         
    ensembl-io/103                                        
    ensembl-io/104                                        
    ensembl-killlist/69                                   
    ensembl-killlist/91                                   
    ensembl-killlist/92                                   
    ensembl-killlist/93                                   
    ensembl-killlist/103                                  
    ensembl-killlist/104                                  
    ensembl-metadata/69                                   
    ensembl-metadata/91                                   
    ensembl-metadata/92                                   
    ensembl-metadata/93                                   
    ensembl-metadata/103                                  
    ensembl-metadata/104                                  
    ensembl-notebook/latest                               
    ensembl-orm/69                                        
    ensembl-orm/91                                        
    ensembl-orm/92                                        
    ensembl-orm/93                                        
    ensembl-orm/103                                       
    ensembl-orm/104                                       
    ensembl-pipeline/69                                   
    ensembl-pipeline/91                                   
    ensembl-pipeline/92                                   
    ensembl-pipeline/93                                   
    ensembl-pipeline/103                                  
    ensembl-pipeline/104                                  
    ensembl-production-api/69                             
    ensembl-production-api/91                             
    ensembl-production-api/92                             
    ensembl-production-api/93                             
    ensembl-production-api/103                            
    ensembl-production-api/104                            
    ensembl-production/69                                 
    ensembl-production/91                                 
    ensembl-production/92                                 
    ensembl-production/93                                 
    ensembl-production/103                                
    ensembl-production/104                                
    ensembl-taxonomy/69                                   
    ensembl-taxonomy/91                                   
    ensembl-taxonomy/92                                   
    ensembl-taxonomy/93                                   
    ensembl-taxonomy/103                                  
    ensembl-taxonomy/104                                  
    ensembl-tools/69                                      
    ensembl-tools/91                                      
    ensembl-tools/92                                      
    ensembl-tools/93                                      
    ensembl-tools/103                                     
    ensembl-tools/104                                     
    ensembl-variation/69                                  
    ensembl-variation/91                                  
    ensembl-variation/92                                  
    ensembl-variation/93                                  
    ensembl-variation/103                                 
    ensembl-variation/104                                 
    ensembl-vep/69                                        
    ensembl-vep/91                                        
    ensembl-vep/92                                        
    ensembl-vep/93                                        
    ensembl-vep/103                                       
    ensembl-vep/104                                       
    ensembl/69                                            
    ensembl/91                                            
    ensembl/92                                            
    ensembl/93                                            
    ensembl/103                                           
    ensembl/104                                           
    ensemblgenomes-api/91                                 
    entrez-direct/13.8.20200819                           
    ericscript/0.5.5                                      
    EVidenceModeler/1.1.1                                 
    evigene/02-11-2017                                    
    evigene/18-01-2018                                    
    evigene/18-09-2013                                    
    evigene/20-05-2020                                    
    evigene/30-07-2021                                    
    exiftool/11.96                                        
    exonerate/2.4.0                                       
    FALCON/1.7.4                                          
    fast-gbs/2016.12.14                                   
    fast-gbs/2017.01.12                                   
    fasta/35.4.12                                         
    fasta/36.3.8g                                         
    fastp/0.12.5                                          
    fastp/0.19.4                                          
    fastp/0.20.0                                          
    fastp/0.23.2                                          
    fastq_screen/v0.4.4                                   
    fastq_screen/v0.5.2                                   
    fastq_screen/v0.11.1                                  
    fastq_screen/v0.14.0                                  
    FastQC/0.11.1                                         
    FastQC/0.11.2                                         
    FastQC/0.11.7                                         
    faststructure/1.0                                     
    FastTree/2.1.10                                       
    fastx_toolkit/0.0.13                                  
    FGMP/1.0                                              
    filtlong/0.2.0                                        
    FLASH/1.2.11                                          
    flye/2.4.2                                            
    flye/2.5                                              
    flye/2.7.1                                            
    flye/2.8.3                                            
    freebayes/1.1.0                                       
    freebayes/1.3.1                                       
    freebayes/1.3.4                                       
    freebayes/1.3.6                                       
    freebayes/v1.0.2-16-gd466dde                          
    freetype/2.9                                          
    GapFiller/v1.10                                       
    GARM/0.7.4                                            
    GATK/1.0                                              
    GATK/3.7                                              
    GATK/3.8.0                                            
    GATK/4.2.6.1                                          
    Gblocks/0.91b                                         
    gdal/2.4.0                                            
    GEM/20130406-045632                                   
    GeMoMa/1.4.2                                          
    GeMoMa/1.6.4                                          
    GeMoMa/1.9                                            
    geneid/v1.4.4                                         
    GeneMark/4.21                                         
    GeneMark/4.33                                         
    GeneMark/4.56                                         
    genomethreader/1.7.0                                  
    genometools/1.5.10                                    
    getorganelle/1.6.2e                                   
    gffcompare/0.12.2                                     
    gffread/0.9.6                                         
    gffread/0.12.7                                        
    git-annex/6.20160613-g35dbe35                         
    git-lfs/2.3.0                                         
    git/2.11.0                                            
    git/2.12.2                                            
    git/2.14.1                                            
    [90;47mgit/2.21.0[0m                                            
    gitflow/15aab26                                       
    glnexus/1.4.3                                         
    globus-cli/1.2.2                                      
    globus-cli/1.6.0                                      
    gmap/2016-06-09                                       
    gmap/2017-06-20                                       
    gmap/2017-09-30                                       
    gmap/2018-03-01                                       
    gmap/2018-03-25                                       
    gmap/2018-05-11                                       
    gmap/2018-05-30                                       
    gmap/2021-12-12                                       
    gmato/v1.2                                            
    GMcloser/1.6.2                                        
    golang/1.9.7                                          
    golang/1.14.2                                         
    GraPhlAn/1.1.3                                        
    GroIMP/1.5                                            
    gromacs/2018                                          
    gromacs/2018.1                                        
    gromacs/2018.2                                        
    gromacs/2018.3                                        
    gromacs/2018.4                                        
    gromacs/2018.5                                        
    gromacs/2019                                          
    gromacs/2022.4                                        
    guppy/3.2.4                                           
    guppy/3.4.4                                           
    guppy/3.5.2                                           
    guppy/3.6.1                                           
    guppy/4.2.2                                           
    guppy/4.4.1                                           
    guppy/5.0.7                                           
    guppy/6.0.1                                           
    guppy/6.3.4                                           
    guppy/6.4.6                                           
    guppy/6.4.6-gpu                                       
    hagfish/1_May_2013                                    
    hagfish/05d08d1                                       
    hapcol/97d4a5e                                        
    hapcompass/0.8.2                                      
    HapCUT2/0121162                                       
    Haplosim/ae652a2                                      
    Haplosim/bd39c6f                                      
    HapTree/1.0                                           
    hclust2/1.0.0                                         
    hdf5/1.8.17                                           
    HiC-pro/2.11.1                                        
    hicup/0.5.9                                           
    hicup/0.7.2                                           
    hisat2/2.1.0                                          
    hisat2/2.2.0                                          
    hisat2/2.2.1                                          
    hmmer/3.0                                             
    hmmer/3.1b1                                           
    hmmer/3.1b2                                           
    hmmer/3.3                                             
    HTSeq/0.6.1                                           
    HTSeq/0.7.2                                           
    HTSeq/0.9.1                                           
    htslib/1.3.1                                          
    htslib/1.7                                            
    htslib/1.9                                            
    htslib/1.10.2                                         
    htslib/1.12                                           
    htslib/1.15.1                                         
    htslib/1.16                                           
    hub/2.8.4                                             
    humann2/0.11.1                                        
    humann2/2.8.1                                         
    humann3/0.0                                           
    iCommands/4.1.8                                       
    idba/a1bafe6                                          
    idr/2.0.4.2                                           
    IGV/2.3.93                                            
    ImageMagick/7.1.0.52                                  
    infernal/1.1.2                                        
    iqtree/1.6.11                                         
    iqtree/2.1.2                                          
    JAFFA/2.1                                             
    JAGS/4.0.0                                            
    JAGS/4.2.0                                            
    java/1.7.0                                            
    java/1.8.0                                            
    jcvi/0.7.3                                            
    jcvi/0.7.7                                            
    jcvi/0.8.12                                           
    jellyfish/1.1.10                                      
    jellyfish/2.1.3                                       
    jellyfish/2.2.10                                      
    jmodeltest/2.1.10                                     
    jq/1.6                                                
    kat/2.3.1                                             
    kat/2.4.1                                             
    kentUtils/302.1                                       
    khmer/2.0                                             
    KMA/1.2.4                                             
    KMC/3.0.0                                             
    kneaddata/0.6.1                                       
    kraken-biom/1.2.0                                     
    kraken/0.10.5                                         
    kraken/1.0                                            
    kraken/1.1                                            
    Krona/2.7                                             
    LACHESIS/20150929                                     
    last/770                                              
    last/1179                                             
    lastz/1.02.00                                         
    lazydocker/0.12                                       
    LDhat/81596e2                                         
    links/v1.8.5                                          
    links/v1.8.6                                          
    LocHap/2.0                                            
    LoRDEC/0.9                                            
    luarocks/2.4.1                                        
    lumpy-sv/0.2.13                                       
    MACS2/2.1.1                                           
    mafft/7.307                                           
    mandalorion-episode-ii/6219d58                        
    mapcomp/1.0                                           
    MAPGD/0.4.26                                          
    MAPGD/0.5                                             
    mapgd/d3edee2                                         
    mash/2.2.2                                            
    mason/0.1.2                                           
    MaSuRCA/3.2.2                                         
    MaSuRCA/3.2.3                                         
    MaSuRCA/3.2.4                                         
    MaSuRCA/3.2.8                                         
    MaSuRCA/3.3.3                                         
    MaSuRCA/4.0.4                                         
    mauve/2015.02.13                                      
    maxbin/2.2.7                                          
    mchap/0.8.0                                           
    mcl/14-137                                            
    mcscan/0.8                                            
    MECAT/3898797                                         
    megahit/1.1.1                                         
    megahit/1.1.3                                         
    megahit/1.2.6                                         
    megahit/1.2.9                                         
    meme/4.11.2                                           
    Meraculous/2.2.4                                      
    merqury/1.3                                           
    Metaassembler/1.5                                     
    metabat/0.32.4                                        
    metabat2/2.15                                         
    metabat2/2.15-3-g367a7ef                              
    metamaps/0.1                                          
    metaphlan2/2.6.0                                      
    metaphlan2/2.96.1                                     
    microbiome_helper/4330e63                             
    mikado/1.1                                            
    miniasm/0.2                                           
    miniasm/55cf018                                       
    miniconda2/4.3.13                                     
    minimap2/2.9                                          
    minimap2/2.17                                         
    minimap2/2.22                                         
    mira/4.0.2                                            
    miRanda/3.3a                                          
    mitoz/2.3                                             
    mplus/0.1                                             
    mrbayes/3.2.7                                         
    mrbayes/3.2.7a                                        
    mrbayes/3.2.7a-gpu                                    
    msms/3.2rc_163                                        
    multiqc/1.0                                           
    multiqc/1.2                                           
    multiqc/1.3                                           
    multiqc/1.5                                           
    multiqc/1.6                                           
    multiqc/1.7                                           
    multiqc/1.8                                           
    multiqc/1.9                                           
    multiqc/1.11                                          
    MUMmer/3.23                                           
    muscle/3.8.1551                                       
    muscle/4.0.170                                        
    nanopack/1.0.0                                        
    nanopack/1.1.1                                        
    nanosv/1.2.4                                          
    ncbi-blast/2.2.25                                     
    ncbi-blast/2.2.30                                     
    ncbi-blast/2.6.0                                      
    ncbi-blast/2.10.1                                     
    ncbi-blast/2.11.0                                     
    ncbi-genome-download/0.2.12                           
    NetLogo/6.0.4                                         
    newbler/2.5.3                                         
    newbler/2.7                                           
    newbler/2.9                                           
    nextclip/v1.3.1                                       
    nextflow/20.07.1                                      
    nextflow/20.10.0                                      
    nextflow/21.04.1                                      
    nextflow/21.10.0                                      
    nextflow/22.04.5                                      
    nextflow/22.10.4                                      
    NextGenMap/v0.5.5                                     
    nextgenmap/v0.5.5                                     
    ngmlr/0.2.7                                           
    NovoGraph/1.0.0                                       
    NOVOPlasty/2.7.2                                      
    NPStat/v1                                             
    nQuire/a990a88                                        
    NSEG/2018-05-30                                       
    nullarbor/1.41                                        
    NxTrim/0.4.2                                          
    NxTrim/v0.4.1-0f17575                                 
    oases/0.2.09                                          
    obitools/1.2.11                                       
    octave/4.2.2                                          
    octave/4.4.1                                          
    octopus/0.7.4                                         
    omni-c/04734cc                                        
    openbugs/3.2.3                                        
    opendronemap/0.4.0                                    
    opendronemap/0.4.1                                    
    openlava/3.2                                          
    openmpi/1.8.8                                         
    openmpi/4.0.2                                         
    OPERA-LG/v2.0.6                                       
    ORA/2.0.0                                             
    orthofinder/2.3.1                                     
    orthofinder/2.5.4                                     
    orthomcl/2.0.9                                        
    PAML/4.9i                                             
    pandaseq/2.10                                         
    [90;47mpandoc/1.19.2[0m                                         
    PASA/2.0.2                                            
    PASA/2.1.0                                            
    PASA/2.2.0                                            
    PASA/2.3.3                                            
    patman/1.2.2                                          
    pblat/2.0                                             
    pblat/2.1                                             
    PBSIM/308622d                                         
    PBSuite/15.8.24                                       
    PBSuite/17.05.09-dbrowneup                            
    pbsv/2.4.0                                            
    pcl/1.8.1                                             
    pcl/1.9.0                                             
    pcl/1.9.1                                             
    PedigreeSim/v2.0                                      
    PEPPER/0.4                                            
    perl-utils/default                                    
    perl/5.8.9                                            
    perl/5.8.9-thread-multi                               
    perl/5.10.1                                           
    perl/5.10.1-thread-multi                              
    perl/5.12.5                                           
    perl/5.12.5-thread-multi                              
    perl/5.14.4                                           
    perl/5.14.4-thread-multi                              
    perl/5.16.3                                           
    perl/5.16.3-thread-multi                              
    perl/5.18.4                                           
    perl/5.20.3                                           
    perl/5.20.3-thread-multi                              
    perl/5.22.2                                           
    perl/5.22.2-thread-multi                              
    perl/5.24.0                                           
    perl/5.24.0-thread-multi                              
    perl/5.24.1                                           
    perl/5.24.1-thread-multi                              
    perl/5.26.0                                           
    perl/5.26.0-thread-multi                              
    perl/5.28.0                                           
    perl/5.28.0-thread-multi                              
    perl/5.30.2                                           
    perl/5.30.2-thread-multi                              
    [90;47mperl/5.36.0[0m                                           
    perl/5.36.0-thread-multi                              
    perl/bio-extras                                       
    perl/core                                             
    perl/ensembl                                          
    perl/jupyterhub                                       
    [90;47mperlbrew/0.76[0m                                         
    pfr-python2/2.7.13                                    
    pfr-python3/3.6.1                                     
    pfr-python3/3.6.5                                     
    pfr-python3/3.6.6                                     
    pfr-python3/3.7.7                                     
    pfr-python3/3.9.13                                    
    pgap/6.1                                              
    pgap/6.2                                              
    pggb/0.5.3                                            
    phantompeakqualtools/1.2.2                            
    phylip/3.696                                          
    phylobayes/4.1c                                       
    PhyloPhlan/3.0.2                                      
    PhyloSift/1.0.1                                       
    PhyloSift/singularity-1.0.1                           
    phyml/3.3.20200621                                    
    picard-tools/1.79                                     
    picard-tools/1.112                                    
    picard-tools/2.2.4                                    
    picard-tools/2.9.4                                    
    picard-tools/2.10.1                                   
    picard-tools/2.18.7                                   
    picrust2/2.3.0                                        
    pilon/1.18                                            
    pilon/1.20                                            
    pilon/1.23                                            
    pinfish/0.1.0                                         
    platanus/1.2.4                                        
    platanus_trim/1.0.7                                   
    Platypus/0.8.1                                        
    plink/1.07                                            
    plink/1.90b6.5                                        
    plink2/v2.00a2lm                                      
    plncpro/1.1                                           
    polyorigin/0.5.3                                      
    popoolation2/1201                                     
    porechop/0.2.3                                        
    portcullis/1.1.0                                      
    portcullis/1.1.1                                      
    portcullis/1.1.2                                      
    [90;47mpowerPl[0;46mant/core[0m                                       
    powerPlant/locate                                     
    pplacer/v1.1.alpha17-6-g5cecf99                       
    ppsPCP/1.0                                            
    primer3/2.2.3                                         
    primer3/2.3.5                                         
    prinseq-lite/0.20.4                                   
    Prodigal/2.6.3                                        
    prodigy/1.10.6                                        
    proj/5.2.0                                            
    prokka/1.11                                           
    prokka/1.13                                           
    prokka/1.14.5                                         
    proteinortho/6.0.15                                   
    purge_haplotigs/1.1.0                                 
    pyarrow/0.16.0                                        
    pycoqc/2.5.0.21                                       
    qctool/2.2.0                                          
    qiime/1.9.1                                           
    QIIME2/2018.2                                         
    QIIME2/2018.11                                        
    QIIME2/2019.1                                         
    QIIME2/2019.1-picrust2                                
    QIIME2/2019.4                                         
    QIIME2/2019.7                                         
    QIIME2/2019.7-picrust2                                
    QIIME2/2019.10                                        
    QIIME2/2020.2                                         
    QIIME2/2020.6                                         
    QIIME2/2020.8                                         
    QIIME2/2020.11                                        
    QIIME2/2020.11-aldex2                                 
    QIIME2/2021.2                                         
    QIIME2/2021.4                                         
    QIIME2/2021.8                                         
    QIIME2/2021.11                                        
    QIIME2/2022.2                                         
    QIIME2/2022.8                                         
    QIIME2/2022.11                                        
    qualimap/v2.2.1                                       
    quast/4.2                                             
    R/3.3.0                                               
    R/3.3.1                                               
    R/3.3.3                                               
    R/3.4.0                                               
    R/3.4.1                                               
    R/3.4.2                                               
    R/3.4.3                                               
    R/3.4.4                                               
    R/3.5.0                                               
    R/3.5.2                                               
    R/3.5.3                                               
    R/3.6.1                                               
    R/3.6.2                                               
    R/3.6.3                                               
    R/4.0.0                                               
    racon/1.3.0                                           
    racon/1.3.1                                           
    racon/1.3.2                                           
    racon/1.3.3                                           
    racon/1.4.0                                           
    racon/1.4.2                                           
    racon/1.4.3                                           
    racon/1.4.7                                           
    ragoo/1.01                                            
    ragoo/1.02                                            
    ragtag/1.0.2                                          
    RAILS/v1.2                                            
    RANBOW/1                                              
    RANBOW/1-temp                                         
    rattle/0.0                                            
    RECON/1.08                                            
    REPCLASS/1.0.1                                        
    RepeatMasker-open/3-3-0                               
    RepeatMasker-open/4-0-3                               
    RepeatMasker-open/4-0-5                               
    RepeatMasker/4.1.2-p1                                 
    RepeatModeler-open/1.0.11                             
    RepeatModeler/1.0.8                                   
    RepeatScout/1.0.5                                     
    REPET/2.5                                             
    REPET/3.0                                             
    rnacocktail/0.2.1                                     
    RSEM/1.3.0                                            
    rtg-tools/3.7.1-eb13bbb                               
    ruby/2.1.9                                            
    ruby/2.2.7                                            
    ruby/2.3.4                                            
    ruby/2.4.1                                            
    sabre/1.000                                           
    salmon/1.1.0                                          
    salmon/1.3.0                                          
    salsa/v2.2                                            
    sambamba/0.8.0                                        
    samtools/0.1.18                                       
    samtools/0.1.19                                       
    samtools/1.1                                          
    samtools/1.2                                          
    samtools/1.3.1                                        
    samtools/1.7                                          
    samtools/1.9                                          
    samtools/1.10                                         
    samtools/1.11                                         
    samtools/1.12                                         
    samtools/1.16                                         
    ScanIndel/1.2dev                                      
    SDhap/56d7678                                         
    seqkit/0.7.0                                          
    seqmagick/0.8.0                                       
    seqtk/1.2                                             
    sex-detector-plusplus/00f7d723                        
    sga/0.9.19                                            
    sga/0.9.35                                            
    sga/0.10.10-2                                         
    sga/0.10.13                                           
    sga/0.10.15                                           
    SGSGeneLoss/0.1                                       
    singularity/2.4.2                                     
    singularity/2.5.1                                     
    singularity/3                                         
    singularity/3.10.3                                    
    slim/3.1                                              
    slim/3.4+1c85d00                                      
    slim/3.5                                              
    [90;47mslurm-utils/latest[0m                                    
    [90;47mSlurm/2[0;46m1.08.8-2[0m                                       
    smalt/0.7.6                                           
    SMRTtools/10.2.1.143962                               
    snakemake/5.10.0                                      
    snakemake/5.30.1                                      
    snakemake/6.15.3                                      
    snap/1.0beta.18                                       
    snapr/0.16alpha.51                                    
    sniffles/1.0.11                                       
    sniffles/1.0.12a                                      
    snipar/0.0.13                                         
    SnpEff/4.3t                                           
    SNPhylo/20140701                                      
    SNPhylo/20160204                                      
    SOAPdenovo-Trans/1.03                                 
    SOAPdenovo/1.05                                       
    SOAPdenovo/2.04                                       
    software/experimental                                 
    SolexaQA/3.1.5                                        
    sortmerna/2.1                                         
    sortmerna/3.0.3                                       
    sortmerna/4.2.0                                       
    sortmerna/4.3.2                                       
    sortmerna/4.3.4                                       
    sortmerna/4.3.6                                       
    sourmash/3.5.0                                        
    SPAdes/3.7.1                                          
    SPAdes/3.10.1                                         
    SPAdes/3.11.1                                         
    SPAdes/3.12.0                                         
    SPAdes/3.13.0                                         
    SPAdes/3.14.0                                         
    SPAdes/3.15.4                                         
    sqlite-tools/3.36.0                                   
    SqueezeMeta/0.4.4                                     
    SqueezeMeta/1.0.0-beta                                
    sratoolkit/2.8.2.1                                    
    sratoolkit/3.0.0                                      
    SSPACE/2.0                                            
    stacks/1.40                                           
    stacks/1.40_withbam                                   
    stacks/2.0                                            
    stacks/2.1                                            
    stacks/2.2                                            
    stacks/2.58                                           
    stamp/2.1.3                                           
    standard-RAxML/8.2.9                                  
    standard-RAxML/8.2.11                                 
    STAR-Fusion/0.8.0                                     
    STAR/2.4.1d                                           
    STAR/2.4.2a                                           
    STAR/2.5.2a                                           
    STAR/2.5.2b                                           
    STAR/2.5.3a                                           
    STAR/2.6.1a                                           
    STAR/2.6.1d                                           
    STAR/2.7.10a                                          
    stringtie/1.3.3b.Linux_x86_64                         
    stringtie/2.2.0                                       
    subread/1.4.5                                         
    subread/1.5.3                                         
    supermagic/1.3-dev                                    
    supernova/1.2.2                                       
    survivor/1.0.5                                        
    SV2/1.4.3.2                                           
    svaba/1.1.3                                           
    svim/1.2.0                                            
    svim/1.4.2                                            
    svtools/0.3.2                                         
    swan/3516c2f                                          
    tabix/0.2.6                                           
    TargQC/1.4.4                                          
    tasr/1.6.2                                            
    tassel/3.0                                            
    tassel/4.0                                            
    tassel/5.0                                            
    tassel/5.2.28                                         
    taxmaps/0.2.1                                         
    tetools/1.1                                           
    [90;47mtexlive/20151117[0m                                      
    tigmint/1.1.2                                         
    tomahawk/0.7.1                                        
    tophat/2.0.13                                         
    tophat/2.1.1                                          
    totalview/2017.2.11                                   
    TransDecoder/3.0.1                                    
    TransDecoder/5.0.1                                    
    TransDecoder/5.5.0                                    
    transrate/1.0.3                                       
    trf/4.07                                              
    trim_galore/0.4.1                                     
    trim_galore/0.4.3                                     
    Trimmomatic/0.36                                      
    trinityrnaseq/2.0.6                                   
    trinityrnaseq/2.2.0                                   
    trinityrnaseq/2.3.2                                   
    trinityrnaseq/2.4.0                                   
    trinityrnaseq/2.5.1                                   
    trinityrnaseq/2.6.5                                   
    trinityrnaseq/2.8.6                                   
    trinityrnaseq/2.9.0                                   
    trinityrnaseq/2.9.1                                   
    trinityrnaseq/2.10.0                                  
    trinityrnaseq/2.13.2                                  
    trinityrnaseq/2.14.0                                  
    trinotate/3.0.2                                       
    trinotate/3.2.0                                       
    trinotate/3.2.2                                       
    tRNAscan-SE/1.3.1                                     
    tRNAscan-SE/2.0                                       
    truvari/2.1.0                                         
    ucsc-pslcdnafilter/324                                
    unicycler/0.4.8                                       
    unixODBC/2.3.0                                        
    variant-effect-predictor/101.0                        
    
    ------------------- [1;94m/software/powerPlant/modulefiles/eb/all[0m --------------------
    binutils/2.34                 GCCcore/10.2.0                     
    binutils/2.34-GCCcore-9.3.0   GCCcore/11.2.0                     
    binutils/2.35                 GCCcore/11.3.0                     
    binutils/2.35-GCCcore-10.2.0  GCCcore/12.2.0                     
    binutils/2.37                 gcccuda/2020a                      
    binutils/2.37-GCCcore-11.2.0  gcccuda/2020b                      
    binutils/2.38                 gettext/0.21                       
    binutils/2.38-GCCcore-11.2.0  help2man/1.47.12-GCCcore-9.3.0     
    binutils/2.38-GCCcore-11.3.0  help2man/1.47.16-GCCcore-10.2.0    
    binutils/2.39                 help2man/1.48.3-GCCcore-11.2.0     
    binutils/2.39-GCCcore-12.2.0  help2man/1.49.2-GCCcore-11.3.0     
    Bison/3.5.3-GCCcore-9.3.0     help2man/1.49.2-GCCcore-12.2.0     
    Bison/3.7.1-GCCcore-10.2.0    Java/17.0.4                        
    Bison/3.7.6-GCCcore-11.2.0    libarchive/3.5.1-GCCcore-11.2.0    
    Bison/3.8.2                   libarchive/3.6.1-GCCcore-11.2.0    
    Bison/3.8.2-GCCcore-11.2.0    libarchive/3.6.1-GCCcore-11.3.0    
    Bison/3.8.2-GCCcore-11.3.0    libffi/3.4.2-GCCcore-11.2.0        
    Bison/3.8.2-GCCcore-12.2.0    libreadline/8.1.2-GCCcore-11.2.0   
    bzip2/1.0.8-GCCcore-11.2.0    M4/1.4.18-GCCcore-9.3.0            
    bzip2/1.0.8-GCCcore-11.3.0    M4/1.4.18-GCCcore-10.2.0           
    CMake/3.22.1-GCCcore-11.2.0   M4/1.4.19                          
    CMake/3.23.1-GCCcore-11.2.0   M4/1.4.19-GCCcore-11.2.0           
    CMake/3.23.1-GCCcore-11.3.0   M4/1.4.19-GCCcore-11.3.0           
    CUDA/11.0.2-GCC-9.3.0         M4/1.4.19-GCCcore-12.2.0           
    CUDA/11.1.1-GCC-10.2.0        ncurses/6.2                        
    CUDA/11.7.0                   ncurses/6.2-GCCcore-11.2.0         
    CUDAcore/11.0.2               ncurses/6.3-GCCcore-11.2.0         
    CUDAcore/11.1.1               ncurses/6.3-GCCcore-11.3.0         
    cURL/7.78.0-GCCcore-11.2.0    OpenMPI/4.1.2-GCC-11.2.0           
    cURL/7.83.0-GCCcore-11.2.0    OpenSSL/1.1                        
    cURL/7.83.0-GCCcore-11.3.0    pkgconf/1.8.0                      
    EasyBuild/4.5.3               pkgconf/1.8.0-GCCcore-11.2.0       
    EasyBuild/4.5.4               Python/3.10.4-GCCcore-11.2.0-bare  
    EasyBuild/4.6.1               SQLite/3.38.3-GCCcore-11.2.0       
    flex/2.6.4                    Tcl/8.6.12-GCCcore-11.2.0          
    flex/2.6.4-GCCcore-9.3.0      UnZip/6.0-GCCcore-11.2.0           
    flex/2.6.4-GCCcore-10.2.0     XZ/5.2.5-GCCcore-11.2.0            
    flex/2.6.4-GCCcore-11.2.0     XZ/5.2.5-GCCcore-11.3.0            
    flex/2.6.4-GCCcore-11.3.0     zlib/1.2.11                        
    flex/2.6.4-GCCcore-12.2.0     zlib/1.2.11-GCCcore-9.3.0          
    GCC/9.3.0                     zlib/1.2.11-GCCcore-10.2.0         
    GCC/10.2.0                    zlib/1.2.11-GCCcore-11.2.0         
    GCC/11.2.0                    zlib/1.2.12                        
    GCC/11.3.0                    zlib/1.2.12-GCCcore-11.2.0         
    GCC/12.2.0                    zlib/1.2.12-GCCcore-11.3.0         
    GCCcore/9.3.0                 zlib/1.2.12-GCCcore-12.2.0         
    
    ----------------- [1;94m/software/powerPlant/modulefiles/eb/compiler[0m -----------------
    GCC/9.3.0   GCC/11.2.0  GCC/12.2.0     GCCcore/10.2.0  GCCcore/11.3.0  
    GCC/10.2.0  GCC/11.3.0  GCCcore/9.3.0  GCCcore/11.2.0  GCCcore/12.2.0  
    
    ------------------ [1;94m/software/powerPlant/modulefiles/eb/devel[0m -------------------
    CMake/3.22.1-GCCcore-11.2.0  ncurses/6.2                   
    CMake/3.23.1-GCCcore-11.3.0  ncurses/6.2-GCCcore-11.2.0    
    M4/1.4.18-GCCcore-9.3.0      ncurses/6.3-GCCcore-11.2.0    
    M4/1.4.18-GCCcore-10.2.0     ncurses/6.3-GCCcore-11.3.0    
    M4/1.4.19                    pkgconf/1.8.0                 
    M4/1.4.19-GCCcore-11.2.0     pkgconf/1.8.0-GCCcore-11.2.0  
    M4/1.4.19-GCCcore-11.3.0     SQLite/3.38.3-GCCcore-11.2.0  
    M4/1.4.19-GCCcore-12.2.0     
    
    ------------------- [1;94m/software/powerPlant/modulefiles/eb/lang[0m -------------------
    Bison/3.5.3-GCCcore-9.3.0   flex/2.6.4-GCCcore-9.3.0           
    Bison/3.7.1-GCCcore-10.2.0  flex/2.6.4-GCCcore-10.2.0          
    Bison/3.7.6-GCCcore-11.2.0  flex/2.6.4-GCCcore-11.2.0          
    Bison/3.8.2                 flex/2.6.4-GCCcore-11.3.0          
    Bison/3.8.2-GCCcore-11.2.0  flex/2.6.4-GCCcore-12.2.0          
    Bison/3.8.2-GCCcore-11.3.0  Java/17.0.4                        
    Bison/3.8.2-GCCcore-12.2.0  Python/3.10.4-GCCcore-11.2.0-bare  
    flex/2.6.4                  Tcl/8.6.12-GCCcore-11.2.0          
    
    ------------------- [1;94m/software/powerPlant/modulefiles/eb/lib[0m --------------------
    libffi/3.4.2-GCCcore-11.2.0       zlib/1.2.11-GCCcore-11.2.0  
    libreadline/8.1.2-GCCcore-11.2.0  zlib/1.2.12                 
    zlib/1.2.11                       zlib/1.2.12-GCCcore-11.2.0  
    zlib/1.2.11-GCCcore-9.3.0         zlib/1.2.12-GCCcore-11.3.0  
    zlib/1.2.11-GCCcore-10.2.0        zlib/1.2.12-GCCcore-12.2.0  
    
    ------------------- [1;94m/software/powerPlant/modulefiles/eb/mpi[0m --------------------
    OpenMPI/4.1.2-GCC-11.2.0  
    
    ------------------ [1;94m/software/powerPlant/modulefiles/eb/system[0m ------------------
    CUDA/11.0.2-GCC-9.3.0   CUDA/11.7.0      CUDAcore/11.1.1  
    CUDA/11.1.1-GCC-10.2.0  CUDAcore/11.0.2  OpenSSL/1.1      
    
    ---------------- [1;94m/software/powerPlant/modulefiles/eb/toolchain[0m -----------------
    gcccuda/2020a  gcccuda/2020b  
    
    ------------------ [1;94m/software/powerPlant/modulefiles/eb/tools[0m -------------------
    binutils/2.34                 EasyBuild/4.5.3                  
    binutils/2.34-GCCcore-9.3.0   EasyBuild/4.5.4                  
    binutils/2.35                 EasyBuild/4.6.1                  
    binutils/2.35-GCCcore-10.2.0  gettext/0.21                     
    binutils/2.37                 help2man/1.47.12-GCCcore-9.3.0   
    binutils/2.37-GCCcore-11.2.0  help2man/1.47.16-GCCcore-10.2.0  
    binutils/2.38                 help2man/1.48.3-GCCcore-11.2.0   
    binutils/2.38-GCCcore-11.2.0  help2man/1.49.2-GCCcore-11.3.0   
    binutils/2.38-GCCcore-11.3.0  help2man/1.49.2-GCCcore-12.2.0   
    binutils/2.39                 libarchive/3.5.1-GCCcore-11.2.0  
    binutils/2.39-GCCcore-12.2.0  libarchive/3.6.1-GCCcore-11.2.0  
    bzip2/1.0.8-GCCcore-11.2.0    libarchive/3.6.1-GCCcore-11.3.0  
    bzip2/1.0.8-GCCcore-11.3.0    UnZip/6.0-GCCcore-11.2.0         
    cURL/7.78.0-GCCcore-11.2.0    XZ/5.2.5-GCCcore-11.2.0          
    cURL/7.83.0-GCCcore-11.2.0    XZ/5.2.5-GCCcore-11.3.0          
    cURL/7.83.0-GCCcore-11.3.0    
    
    Key:
    [90;47mloaded[0m  [1;94mmodulepath[0m  [46msticky[0m  


## 1. Prepare data and directories

Data were sent physically in a hard drive. A working copy has been made inside cfndxa/MarsdenObj1


```bash
cd X201SC20071998-Z01-F001
```


```bash
cd 01.RawData
ls
```

    EC_1  EC_2  EC_3  EC_4	EC_5  EC_6  WC_1  WC_2	WC_3  WC_5  WC_6



```bash
find -type f -exec md5sum "{}" + > checklist.chk
```


```bash
md5sum -c checklist.chk
```

    ./EC_3/EC_3_FKDN220184500-1A_H5CMTDSX3_L1_1.fq.gz: OK
    ./EC_3/MD5.txt: OK
    ./EC_3/EC_3_FKDN220184500-1A_H5CMTDSX3_L1_2.fq.gz: OK
    ./EC_4/EC_4_FKDN220184501-1A_H5K3KDSX3_L4_1.fq.gz: OK
    ./EC_4/EC_4_FKDN220184501-1A_H5K3KDSX3_L4_2.fq.gz: OK
    ./EC_4/MD5.txt: OK
    ./EC_4/EC_4_FKDN220184501-1A_H5GGLDSX3_L4_2.fq.gz: OK
    ./EC_4/EC_4_FKDN220184501-1A_H5GGLDSX3_L4_1.fq.gz: OK
    ./WC_1/MD5.txt: OK
    ./WC_1/WC_1_FKDN220184493-1A_H5CMTDSX3_L1_2.fq.gz: OK
    ./WC_1/WC_1_FKDN220184493-1A_H5CMTDSX3_L1_1.fq.gz: OK
    ./WC_6/WC_6_FKDN220184497-1A_H5GGJDSX3_L3_1.fq.gz: OK
    ./WC_6/MD5.txt: OK
    ./WC_6/WC_6_FKDN220184497-1A_H5GGJDSX3_L3_2.fq.gz: OK
    ./EC_6/MD5.txt: OK
    ./EC_6/EC_6_FKDN220184503-1A_H5CMTDSX3_L1_1.fq.gz: OK
    ./EC_6/EC_6_FKDN220184503-1A_H5CMTDSX3_L1_2.fq.gz: OK
    ./EC_2/MD5.txt: OK
    ./EC_2/EC_2_FKDN220184499-1A_H5GGLDSX3_L4_1.fq.gz: OK
    ./EC_2/EC_2_FKDN220184499-1A_H5GGLDSX3_L4_2.fq.gz: OK
    ./EC_2/EC_2_FKDN220184499-1A_H5K3KDSX3_L4_2.fq.gz: OK
    ./EC_2/EC_2_FKDN220184499-1A_H5K3KDSX3_L4_1.fq.gz: OK
    ./EC_5/MD5.txt: OK
    ./EC_5/EC_5_FKDN220184502-1A_H5CMTDSX3_L1_1.fq.gz: OK
    ./EC_5/EC_5_FKDN220184502-1A_H5CMTDSX3_L1_2.fq.gz: OK
    ./WC_3/MD5.txt: OK
    ./WC_3/WC_3_FKDN220184495-1A_H5CMTDSX3_L1_1.fq.gz: OK
    ./WC_3/WC_3_FKDN220184495-1A_H5CMTDSX3_L1_2.fq.gz: OK
    ./checklist.chk: FAILED
    ./WC_5/MD5.txt: OK
    ./WC_5/WC_5_FKDN220184496-1A_H5CMTDSX3_L1_2.fq.gz: OK
    ./WC_5/WC_5_FKDN220184496-1A_H5CMTDSX3_L1_1.fq.gz: OK
    ./WC_2/WC_2_FKDN220184494-1A_H5CMTDSX3_L1_2.fq.gz: OK
    ./WC_2/MD5.txt: OK
    ./WC_2/WC_2_FKDN220184494-1A_H5CMTDSX3_L1_1.fq.gz: OK
    ./EC_1/EC_1_FKDN220184498-1A_H5CMTDSX3_L1_2.fq.gz: OK
    ./EC_1/MD5.txt: OK
    ./EC_1/EC_1_FKDN220184498-1A_H5CMTDSX3_L1_1.fq.gz: OK
    md5sum: WARNING: 1 computed checksum did NOT match




### Define Project Variables and create analysis directories:


```bash
#Create analysis directories and define project variables

# Define the user as a variable
USER="cfndxa"

# Define the project directory and temp subdirectory as a variable

PROJECT="/workspace/$USER/MarsdenObj1/Sequencing_WGBS"
```


```bash
# Create the project directory

mkdir -p $PROJECT

# Create the temp directory

mkdir -p $TEMP

# Create analysis subdirectories

mkdir -p $PROJECT/000.raw
mkdir -p $PROJECT/001.fastqc_raw
mkdir -p $PROJECT/002.trimmomatic
mkdir -p $PROJECT/003.fastq_trimmomatic
mkdir -p $PROJECT/004.alignments
mkdir -p $PROJECT/005.b.stats_alignments
mkdir -p $PROJECT/005.qc_alignments
mkdir -p $PROJECT/006.deduplication
mkdir -p $PROJECT/007.meth_extraction
mkdir -p $PROJECT/008.methylkit
mkdir -p $PROJECT/099.test
```

    mkdir: missing operand
    Try 'mkdir --help' for more information.



```bash
cd /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS
```

### 1.1 FastQC RAW Data
- The input for this step is the raw data from the provider in FASTQ format
- The output from this step are the HTML FASTQC Reports


```bash
# Define the location for the QC reports:
IN="${PROJECT}/X201SC20071998-Z01-F001/01.RawData"
OUT="${PROJECT}/001.fastqc_raw"

# Define the list of files to process:
FILES=`find -type f -name "*.fq.gz"`

# Load the FastQC module:
module load FastQC

for file in $FILES
    do
        COMMAND="fastqc --nogroup -q -t 2 -o ${OUT} ${file}"
        echo $COMMAND
done | abatch -j ${OUT}/fastqc_raw --time 01:00:00 --mem 1G | sbatch
```

    /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/X201SC20071998-Z01-F001/01.RawData
    /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/001.fastqc_raw
    SBATCH_ARGS: --time 01:00:00 --mem 1G
    JOB_ARRAY_NAME: /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/001.fastqc_raw/fastqc_raw
    GROUP_SIZE: 1
    NUM_COMMANDS: 26
    Submitted batch job 1059579



```bash
module load multiqc
```

    ** INFO ** : singularity has been deprecated - please use apptainer in place.
    
    Loading [1mmultiqc/1.11[22m
      [94mLoading requirement[0m: singularity/3.10.3



```bash
multiqc 001.fastqc_raw -o 001.fastqc_raw -i Fastqc-Raw
```

    
      [34m/[0m[32m/[0m[31m/[0m ]8;id=1678927475.1725929-866276;https://multiqc.info\[1mMultiQC[0m]8;;\ 🔍 [2m| v1.11[0m
    
    [34m|           multiqc[0m | [33mMultiQC Version v1.14 now available![0m
    [34m|           multiqc[0m | Report title: Fastqc-Raw
    [34m|           multiqc[0m | Search path : /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/001.fastqc_raw
    [2K[34m|[0m         [34msearching[0m | [90m━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━[0m [35m100%[0m [32m105/105[0m  0m[0m  
    [?25h[34m|            fastqc[0m | Found 26 reports
    [34m|           multiqc[0m | Compressing plot data
    [34m|           multiqc[0m | Report      : 001.fastqc_raw/Fastqc-Raw_multiqc_report.html
    [34m|           multiqc[0m | Data        : 001.fastqc_raw/Fastqc-Raw_multiqc_report_data
    [34m|           multiqc[0m | MultiQC complete


### 1.2 Merge fastq files from different lanes

Merged files are produced in the current folder and are named as e.g. "EC_1_1.fq.gz" etc


```bash
cd X201SC20071998-Z01-F001/01.RawData
ls
```

    checklist.chk  EC_1  EC_2  EC_3  EC_4  EC_5  EC_6  WC_1  WC_2  WC_3  WC_5  WC_6



```bash
for dir in */*; do 
    dirname=${dir%%/*}; 
    cat $dirname/*1.fq.gz > "${dirname}"_1.fq.gz; 
done
```


```bash
for dir in */*; do 
    dirname=${dir%%/*}; 
    cat $dirname/*2.fq.gz > "${dirname}"_2.fq.gz; 
done
```


```bash
squeue -u cfndxa
```

                 JOBID PARTITION     NAME     USER ST       TIME  NODES NODELIST(REASON)
               5711562    medium [RStudio   cfndxa PD       0:00      1 (Priority)


Move new merged files to 000.raw/merged


```bash
# Define the location for the QC reports:
IN="${PROJECT}/000.raw/merged"
OUT="${PROJECT}/001.fastq_raw_merged"

# Define the list of files to process:
FILES=`find -type f -name "*.fq.gz"`

# Load the FastQC module:
module load FastQC

for file in $FILES
    do
        COMMAND="fastqc --nogroup -q -t 2 -o ${OUT} ${file}"
        echo $COMMAND
done | abatch -j ${OUT}/fastqc_raw --time 01:00:00 --mem 1G | sbatch
```

    SBATCH_ARGS: --time 01:00:00 --mem 1G
    JOB_ARRAY_NAME: /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/001.fastq_raw_merged/fastqc_raw
    GROUP_SIZE: 1
    NUM_COMMANDS: 22
    Submitted batch job 5711591



```bash
multiqc 001.fastq_raw_merged -o 001.fastq_raw_merged -i 001.fastq_raw_merged/Fastqc-Raw
```

## 2. Trimming


```bash
# Run the Trimmomatic program on the filtered data to remove Illumina adapters, homo-polymers, and low quality reads:
  # Note that to do this, it is necessary to edit the file containing the adapter sequences
  # to include all sequences that you wish to remove:
  # This file is called Illumina.fa and is in the 000.raw directory.

IN="${PROJECT}/000.raw/merged"
OUT="${PROJECT}/002.trimmomatic"
UNPAIRED="${OUT}/unpaired"

mkdir -p $IN
mkdir -p $OUT
mkdir -p $UNPAIRED

# Set the path to the adapter file:
CLIP="${OUT}/adapters.fasta"
# Get the files to trim:
# Use echo statements to be sure that the results from awk are what you really want...
FILES=`basename -a ${IN}/*.fq.gz | sed 's/_[1,2].fq.gz//g'|sort -u `
#FILES=`ls ${IN}/*.fastq | awk -F'[_ ]' '{print $1"_"$2"_"$3"_"$4"_"$5"_"$6}' | sort -u`

echo $FILES
module load Trimmomatic

for FILE in $FILES
     do
        In_File1=${IN}/${FILE}_1.fq.gz
        In_File2=${IN}/${FILE}_2.fq.gz
  #      echo $In_File1
  #      echo $In_File2
        Out_PAIRED_1=${OUT}/${FILE}_trimmomatic_R1.fastq
        Out_UNPAIRED_1=${UNPAIRED}/${FILE}_trimmomatic_unpaired_1.fastq
        Out_PAIRED_2=${OUT}/${FILE}_trimmomatic_R2.fastq
        Out_UNPAIRED_2=${UNPAIRED}/${FILE}_trimmomatic_unpaired_2.fastq
  #      echo $Out_PAIRED_1
  #      echo $Out_UNPAIRED_1
  #      echo $Out_PAIRED_2
  #      echo $Out_UNPAIRED_2
        COMMAND="java -jar -Xms8G -Xmx8G \
                 ${TRIMMOMATIC} PE -threads 3 \
                 ${In_File1} ${In_File2} \
                 ${Out_PAIRED_1} ${Out_UNPAIRED_1} ${Out_PAIRED_2} ${Out_UNPAIRED_2} \
                 ILLUMINACLIP:${CLIP}:2:30:10 SLIDINGWINDOW:5:20 MINLEN:50 HEADCROP:10 LEADING:5 TRAILING:5" # headcrop suggested by Novogene due to library construction protocol
       echo $COMMAND
done | abatch -j ${OUT}/trimmomatic-logs --time 01:00:00 --mem 1G | sbatch
```

    EC_1 EC_2 EC_3 EC_4 EC_5 EC_6 WC_1 WC_2 WC_3 WC_5 WC_6
    SBATCH_ARGS: --time 01:00:00 --mem 1G
    JOB_ARRAY_NAME: /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/002.trimmomatic/trimmomatic-logs
    GROUP_SIZE: 1
    NUM_COMMANDS: 11
    Submitted batch job 1059719


### 2.1 FastQC TRIMMED Data
- The input for this step is the raw data from the provider in FASTQ format
- The output from this step are the HTML FASTQC Reports


```bash
 # Define the location for the QC reports:
IN="${PROJECT}/002.trimmomatic"
OUT="${PROJECT}/003.fastq_trimmomatic"

# Define the list of files to process:
FILES=`ls ${IN}/*.fastq`

# Load the FastQC module:
module load FastQC

for file in $FILES
    do
        COMMAND="fastqc --nogroup -q -t 2 -o ${OUT} ${file}"
        echo $COMMAND
done | abatch -j ${OUT}/fastqc-trimmomatic-logs --time 01:00:00 --mem 1G | sbatch
```

    SBATCH_ARGS: --time 01:00:00 --mem 1G
    JOB_ARRAY_NAME: /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/003.fastq_trimmomatic/fastqc-trimmomatic-logs
    GROUP_SIZE: 1
    NUM_COMMANDS: 22
    Submitted batch job 1061325



```bash
module load multiqc
```

    ** INFO ** : singularity has been deprecated - please use apptainer in place.
    
    Loading [1mmultiqc/1.11[22m
      [94mLoading requirement[0m: singularity/3.10.3



```bash
multiqc 003.fastq_trimmomatic -o 003.fastq_trimmomatic -i Fastqc-Trimmed
```

    
      [34m/[0m[32m/[0m[31m/[0m ]8;id=1679006215.2262704-625372;https://multiqc.info\[1mMultiQC[0m]8;;\ 🔍 [2m| v1.11[0m
    
    [34m|           multiqc[0m | [33mMultiQC Version v1.14 now available![0m
    [34m|           multiqc[0m | Report title: Fastqc-Trimmed
    [34m|           multiqc[0m | Search path : /powerplant/workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/003.fastq_trimmomatic
    [2K[34m|[0m         [34msearching[0m | [90m━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━[0m [35m100%[0m [32m87/87[0m  [0m0m  
    [?25h[34m|            fastqc[0m | Found 21 reports
    [34m|           multiqc[0m | Compressing plot data
    [34m|           multiqc[0m | Report      : 003.fastq_trimmomatic/Fastqc-Trimmed_multiqc_report.html
    [34m|           multiqc[0m | Data        : 003.fastq_trimmomatic/Fastqc-Trimmed_multiqc_report_data
    [34m|           multiqc[0m | MultiQC complete


## 3. Alignment Workflow</u>
### 3.1: Index the Genome Using BWA-METH
* The genome was indexed previously when running WGBS pipeline for Obj. 2
* see WGBS-Obj2-Marsden.ipynb

* I had to re-install bwa-meth according to their README file to install toolshed


```bash
cd /workspace/cfndxa
```


```bash
wget https://pypi.python.org/packages/source/t/toolshed/toolshed-0.4.0.tar.gz
tar xzvf toolshed-0.4.0.tar.gz
cd toolshed-0.4.0
python setup.py install --user
```

    --2023-03-17 12:16:34--  https://pypi.python.org/packages/source/t/toolshed/toolshed-0.4.0.tar.gz
    Resolving pypi.python.org (pypi.python.org)... 151.101.164.223, 2a04:4e42:27::223
    Connecting to pypi.python.org (pypi.python.org)|151.101.164.223|:443... connected.
    HTTP request sent, awaiting response... 301 Redirect to Primary Domain
    Location: https://pypi.org/packages/source/t/toolshed/toolshed-0.4.0.tar.gz [following]
    --2023-03-17 12:16:34--  https://pypi.org/packages/source/t/toolshed/toolshed-0.4.0.tar.gz
    Resolving pypi.org (pypi.org)... 151.101.192.223, 151.101.64.223, 151.101.128.223, ...
    Connecting to pypi.org (pypi.org)|151.101.192.223|:443... connected.
    HTTP request sent, awaiting response... 301 Moved Permanently
    Location: https://files.pythonhosted.org/packages/source/t/toolshed/toolshed-0.4.0.tar.gz [following]
    --2023-03-17 12:16:34--  https://files.pythonhosted.org/packages/source/t/toolshed/toolshed-0.4.0.tar.gz
    Resolving files.pythonhosted.org (files.pythonhosted.org)... 151.101.165.63, 2a04:4e42:27::319
    Connecting to files.pythonhosted.org (files.pythonhosted.org)|151.101.165.63|:443... connected.
    HTTP request sent, awaiting response... 302 Found
    Location: https://files.pythonhosted.org/packages/02/a0/d00042b7c86d0a55bad224f7b41e27557fcfad0304750a2e5caf64f38cdd/toolshed-0.4.0.tar.gz [following]
    --2023-03-17 12:16:34--  https://files.pythonhosted.org/packages/02/a0/d00042b7c86d0a55bad224f7b41e27557fcfad0304750a2e5caf64f38cdd/toolshed-0.4.0.tar.gz
    Reusing existing connection to files.pythonhosted.org:443.
    HTTP request sent, awaiting response... 200 OK
    Length: 13566 (13K) [application/octet-stream]
    Saving to: ‘toolshed-0.4.0.tar.gz’
    
    100%[======================================>] 13,566      --.-K/s   in 0s      
    
    2023-03-17 12:16:34 (178 MB/s) - ‘toolshed-0.4.0.tar.gz’ saved [13566/13566]
    
    toolshed-0.4.0/
    toolshed-0.4.0/ez_setup.py
    toolshed-0.4.0/toolshed/
    toolshed-0.4.0/toolshed/files.py
    toolshed-0.4.0/toolshed/fmt.py
    toolshed-0.4.0/toolshed/pool.py
    toolshed-0.4.0/toolshed/__init__.py
    toolshed-0.4.0/toolshed/optimize.py
    toolshed-0.4.0/toolshed.egg-info/
    toolshed-0.4.0/toolshed.egg-info/top_level.txt
    toolshed-0.4.0/toolshed.egg-info/SOURCES.txt
    toolshed-0.4.0/toolshed.egg-info/PKG-INFO
    toolshed-0.4.0/toolshed.egg-info/dependency_links.txt
    toolshed-0.4.0/toolshed.egg-info/entry_points.txt
    toolshed-0.4.0/toolshed.egg-info/not-zip-safe
    toolshed-0.4.0/PKG-INFO
    toolshed-0.4.0/setup.cfg
    toolshed-0.4.0/README.rst
    toolshed-0.4.0/setup.py
    toolshed-0.4.0/NEWS.txt
    toolshed-0.4.0/MANIFEST.in
    running install
    /software/pfr-python3/3.9.13/lib/python3.9/site-packages/setuptools/command/install.py:34: SetuptoolsDeprecationWarning: setup.py install is deprecated. Use build and pip and other standards-based tools.
      warnings.warn(
    /software/pfr-python3/3.9.13/lib/python3.9/site-packages/setuptools/command/easy_install.py:144: EasyInstallDeprecationWarning: easy_install command is deprecated. Use build and pip and other standards-based tools.
      warnings.warn(
    running bdist_egg
    running egg_info
    writing toolshed.egg-info/PKG-INFO
    writing dependency_links to toolshed.egg-info/dependency_links.txt
    writing entry points to toolshed.egg-info/entry_points.txt
    writing top-level names to toolshed.egg-info/top_level.txt
    reading manifest file 'toolshed.egg-info/SOURCES.txt'
    reading manifest template 'MANIFEST.in'
    writing manifest file 'toolshed.egg-info/SOURCES.txt'
    installing library code to build/bdist.linux-x86_64/egg
    running install_lib
    running build_py
    creating build
    creating build/lib
    creating build/lib/toolshed
    copying toolshed/pool.py -> build/lib/toolshed
    copying toolshed/optimize.py -> build/lib/toolshed
    copying toolshed/files.py -> build/lib/toolshed
    copying toolshed/__init__.py -> build/lib/toolshed
    copying toolshed/fmt.py -> build/lib/toolshed
    creating build/bdist.linux-x86_64
    creating build/bdist.linux-x86_64/egg
    creating build/bdist.linux-x86_64/egg/toolshed
    copying build/lib/toolshed/pool.py -> build/bdist.linux-x86_64/egg/toolshed
    copying build/lib/toolshed/optimize.py -> build/bdist.linux-x86_64/egg/toolshed
    copying build/lib/toolshed/files.py -> build/bdist.linux-x86_64/egg/toolshed
    copying build/lib/toolshed/__init__.py -> build/bdist.linux-x86_64/egg/toolshed
    copying build/lib/toolshed/fmt.py -> build/bdist.linux-x86_64/egg/toolshed
    byte-compiling build/bdist.linux-x86_64/egg/toolshed/pool.py to pool.cpython-39.pyc
    byte-compiling build/bdist.linux-x86_64/egg/toolshed/optimize.py to optimize.cpython-39.pyc
    byte-compiling build/bdist.linux-x86_64/egg/toolshed/files.py to files.cpython-39.pyc
    byte-compiling build/bdist.linux-x86_64/egg/toolshed/__init__.py to __init__.cpython-39.pyc
    byte-compiling build/bdist.linux-x86_64/egg/toolshed/fmt.py to fmt.cpython-39.pyc
    creating build/bdist.linux-x86_64/egg/EGG-INFO
    copying toolshed.egg-info/PKG-INFO -> build/bdist.linux-x86_64/egg/EGG-INFO
    copying toolshed.egg-info/SOURCES.txt -> build/bdist.linux-x86_64/egg/EGG-INFO
    copying toolshed.egg-info/dependency_links.txt -> build/bdist.linux-x86_64/egg/EGG-INFO
    copying toolshed.egg-info/entry_points.txt -> build/bdist.linux-x86_64/egg/EGG-INFO
    copying toolshed.egg-info/not-zip-safe -> build/bdist.linux-x86_64/egg/EGG-INFO
    copying toolshed.egg-info/top_level.txt -> build/bdist.linux-x86_64/egg/EGG-INFO
    creating dist
    creating 'dist/toolshed-0.4.0-py3.9.egg' and adding 'build/bdist.linux-x86_64/egg' to it
    removing 'build/bdist.linux-x86_64/egg' (and everything under it)
    Processing toolshed-0.4.0-py3.9.egg
    creating /home/cfndxa/.local/lib/python3.9/site-packages/toolshed-0.4.0-py3.9.egg
    Extracting toolshed-0.4.0-py3.9.egg to /home/cfndxa/.local/lib/python3.9/site-packages
    Adding toolshed 0.4.0 to easy-install.pth file
    Installing toolshed script to /home/cfndxa/.local/bin
    
    Installed /home/cfndxa/.local/lib/python3.9/site-packages/toolshed-0.4.0-py3.9.egg
    Processing dependencies for toolshed==0.4.0
    Finished processing dependencies for toolshed==0.4.0



```bash
wget https://github.com/brentp/bwa-meth/archive/master.zip
unzip master.zip
cd bwa-meth-master/
python setup.py install --user
```

    --2023-03-17 12:17:28--  https://github.com/brentp/bwa-meth/archive/master.zip
    Resolving github.com (github.com)... 20.248.137.48
    Connecting to github.com (github.com)|20.248.137.48|:443... connected.
    HTTP request sent, awaiting response... 302 Found
    Location: https://codeload.github.com/brentp/bwa-meth/zip/refs/heads/master [following]
    --2023-03-17 12:17:28--  https://codeload.github.com/brentp/bwa-meth/zip/refs/heads/master
    Resolving codeload.github.com (codeload.github.com)... 20.248.137.55
    Connecting to codeload.github.com (codeload.github.com)|20.248.137.55|:443... connected.
    HTTP request sent, awaiting response... 200 OK
    Length: unspecified [application/zip]
    Saving to: ‘master.zip’
    
        [    <=>                                ] 8,823,421   10.6MB/s   in 0.8s   
    
    2023-03-17 12:17:30 (10.6 MB/s) - ‘master.zip’ saved [8823421]
    
    Archive:  master.zip
    af57384e25d4910e81556736a998c1891822d0d2
       creating: bwa-meth-master/
      inflating: bwa-meth-master/.gitignore  
      inflating: bwa-meth-master/LICENSE  
      inflating: bwa-meth-master/README.md  
      inflating: bwa-meth-master/bwameth.py  
       creating: bwa-meth-master/compare/
      inflating: bwa-meth-master/compare/README.md  
      inflating: bwa-meth-master/compare/cmp-bis2.sh  
      inflating: bwa-meth-master/compare/common.sh  
       creating: bwa-meth-master/compare/data/
      inflating: bwa-meth-master/compare/data/mm10.capture-regions.bed.gz  
      inflating: bwa-meth-master/compare/data/real-quals.txt  
      inflating: bwa-meth-master/compare/data/real-trim-quals.txt  
      inflating: bwa-meth-master/compare/data/sim-quals.txt  
      inflating: bwa-meth-master/compare/data/sim-trim-quals.txt  
      inflating: bwa-meth-master/compare/plots.sh  
      inflating: bwa-meth-master/compare/run-bis1.sh  
      inflating: bwa-meth-master/compare/run-bis2.sh  
      inflating: bwa-meth-master/compare/run-bison.sh  
      inflating: bwa-meth-master/compare/run-bsmap.sh  
      inflating: bwa-meth-master/compare/run-bsmooth.sh  
      inflating: bwa-meth-master/compare/run-bwa.sh  
      inflating: bwa-meth-master/compare/run-gnumapbs.sh  
      inflating: bwa-meth-master/compare/run-gsnap.sh  
      inflating: bwa-meth-master/compare/run-last.sh  
      inflating: bwa-meth-master/compare/search-bis2.sh  
       creating: bwa-meth-master/compare/src/
      inflating: bwa-meth-master/compare/src/bsmooth-adjust-crick.py  
      inflating: bwa-meth-master/compare/src/extract-read.py  
      inflating: bwa-meth-master/compare/src/gen-simulated.sh  
      inflating: bwa-meth-master/compare/src/gsnap-meth.py  
      inflating: bwa-meth-master/compare/src/last-bisulfite-paired.sh  
      inflating: bwa-meth-master/compare/src/parse-time-mem.py  
      inflating: bwa-meth-master/compare/src/plot-quals-bw.R  
      inflating: bwa-meth-master/compare/src/plot-quals.R  
      inflating: bwa-meth-master/compare/src/sim-roc.py  
      inflating: bwa-meth-master/compare/src/target-roc.py  
      inflating: bwa-meth-master/compare/src/trim.sh  
       creating: bwa-meth-master/example/
      inflating: bwa-meth-master/example/README.md  
      inflating: bwa-meth-master/example/ref.fa  
     extracting: bwa-meth-master/example/t_R1.fastq.gz  
     extracting: bwa-meth-master/example/t_R2.fastq.gz  
      inflating: bwa-meth-master/example/test.sh  
      inflating: bwa-meth-master/ez_setup.py  
       creating: bwa-meth-master/paper/
      inflating: bwa-meth-master/paper/Makefile  
      inflating: bwa-meth-master/paper/bioinfo.cls  
      inflating: bwa-meth-master/paper/document.bib  
      inflating: bwa-meth-master/paper/document.tex  
      inflating: bwa-meth-master/paper/natbib.bst  
      inflating: bwa-meth-master/paper/natbib.sty  
      inflating: bwa-meth-master/paper/noerrorsim-quals.eps  
      inflating: bwa-meth-master/paper/noerrorsim-trim-quals.eps  
      inflating: bwa-meth-master/paper/real-bwa-strand.eps  
      inflating: bwa-meth-master/paper/real-quals.eps  
      inflating: bwa-meth-master/paper/real-trim-quals.eps  
      inflating: bwa-meth-master/paper/sim-quals.eps  
      inflating: bwa-meth-master/paper/sim-trim-quals.eps  
      inflating: bwa-meth-master/paper/supplement.tex  
     extracting: bwa-meth-master/requirements.txt  
       creating: bwa-meth-master/scripts/
      inflating: bwa-meth-master/scripts/bsseq-caller.R  
      inflating: bwa-meth-master/scripts/tabulate-methylation.py  
      inflating: bwa-meth-master/setup.py  
    running install
    /software/pfr-python3/3.9.13/lib/python3.9/site-packages/setuptools/command/install.py:34: SetuptoolsDeprecationWarning: setup.py install is deprecated. Use build and pip and other standards-based tools.
      warnings.warn(
    /software/pfr-python3/3.9.13/lib/python3.9/site-packages/setuptools/command/easy_install.py:144: EasyInstallDeprecationWarning: easy_install command is deprecated. Use build and pip and other standards-based tools.
      warnings.warn(
    running bdist_egg
    running egg_info
    creating bwameth.egg-info
    writing bwameth.egg-info/PKG-INFO
    writing dependency_links to bwameth.egg-info/dependency_links.txt
    writing requirements to bwameth.egg-info/requires.txt
    writing top-level names to bwameth.egg-info/top_level.txt
    writing manifest file 'bwameth.egg-info/SOURCES.txt'
    reading manifest file 'bwameth.egg-info/SOURCES.txt'
    adding license file 'LICENSE'
    writing manifest file 'bwameth.egg-info/SOURCES.txt'
    installing library code to build/bdist.linux-x86_64/egg
    running install_lib
    running build_py
    creating build
    creating build/lib
    copying bwameth.py -> build/lib
    creating build/bdist.linux-x86_64
    creating build/bdist.linux-x86_64/egg
    copying build/lib/bwameth.py -> build/bdist.linux-x86_64/egg
    byte-compiling build/bdist.linux-x86_64/egg/bwameth.py to bwameth.cpython-39.pyc
    creating build/bdist.linux-x86_64/egg/EGG-INFO
    installing scripts to build/bdist.linux-x86_64/egg/EGG-INFO/scripts
    running install_scripts
    running build_scripts
    creating build/scripts-3.9
    copying and adjusting bwameth.py -> build/scripts-3.9
    changing mode of build/scripts-3.9/bwameth.py from 664 to 775
    creating build/bdist.linux-x86_64/egg/EGG-INFO/scripts
    copying build/scripts-3.9/bwameth.py -> build/bdist.linux-x86_64/egg/EGG-INFO/scripts
    changing mode of build/bdist.linux-x86_64/egg/EGG-INFO/scripts/bwameth.py to 775
    copying bwameth.egg-info/PKG-INFO -> build/bdist.linux-x86_64/egg/EGG-INFO
    copying bwameth.egg-info/SOURCES.txt -> build/bdist.linux-x86_64/egg/EGG-INFO
    copying bwameth.egg-info/dependency_links.txt -> build/bdist.linux-x86_64/egg/EGG-INFO
    copying bwameth.egg-info/requires.txt -> build/bdist.linux-x86_64/egg/EGG-INFO
    copying bwameth.egg-info/top_level.txt -> build/bdist.linux-x86_64/egg/EGG-INFO
    zip_safe flag not set; analyzing archive contents...
    __pycache__.bwameth.cpython-39: module references __file__
    creating dist
    creating 'dist/bwameth-0.2.6-py3.9.egg' and adding 'build/bdist.linux-x86_64/egg' to it
    removing 'build/bdist.linux-x86_64/egg' (and everything under it)
    Processing bwameth-0.2.6-py3.9.egg
    creating /home/cfndxa/.local/lib/python3.9/site-packages/bwameth-0.2.6-py3.9.egg
    Extracting bwameth-0.2.6-py3.9.egg to /home/cfndxa/.local/lib/python3.9/site-packages
    Adding bwameth 0.2.6 to easy-install.pth file
    Installing bwameth.py script to /home/cfndxa/.local/bin
    
    Installed /home/cfndxa/.local/lib/python3.9/site-packages/bwameth-0.2.6-py3.9.egg
    Processing dependencies for bwameth==0.2.6
    Searching for toolshed>=0.4.5
    Reading https://pypi.org/simple/toolshed/
    /software/pfr-python3/3.9.13/lib/python3.9/site-packages/pkg_resources/__init__.py:123: PkgResourcesDeprecationWarning:  is an invalid version and will not be supported in a future release
      warnings.warn(
    Downloading https://files.pythonhosted.org/packages/08/bd/d6259c8d882f6783fdfe69bfaed628afb1ddd291f8a1ac6176d27c62860c/toolshed-0.4.6.tar.gz#sha256=23a31c177bf84244b30a9f12c7a8a17a66a2d63043ead0460c31b9ff42f9fb93
    Best match: toolshed 0.4.6
    Processing toolshed-0.4.6.tar.gz
    Writing /tmp/easy_install-8kmxx4nt/toolshed-0.4.6/setup.cfg
    Running toolshed-0.4.6/setup.py -q bdist_egg --dist-dir /tmp/easy_install-8kmxx4nt/toolshed-0.4.6/egg-dist-tmp-bn0i7rg1
    /software/pfr-python3/3.9.13/lib/python3.9/site-packages/setuptools/command/install.py:34: SetuptoolsDeprecationWarning: setup.py install is deprecated. Use build and pip and other standards-based tools.
      warnings.warn(
    creating /home/cfndxa/.local/lib/python3.9/site-packages/toolshed-0.4.6-py3.9.egg
    Extracting toolshed-0.4.6-py3.9.egg to /home/cfndxa/.local/lib/python3.9/site-packages
    Removing toolshed 0.4.0 from easy-install.pth file
    Adding toolshed 0.4.6 to easy-install.pth file
    Installing toolshed script to /home/cfndxa/.local/bin
    
    Installed /home/cfndxa/.local/lib/python3.9/site-packages/toolshed-0.4.6-py3.9.egg
    Finished processing dependencies for bwameth==0.2.6



```bash
export "PATH=$PATH:/home/cfndxa/.local/bin"
echo $PATH
```

    /software/bioinformatics/bwa-0.7.17:/software/samtools/1.16/bin:/software/pfr-python3/3.9.13/bin:/software/bioinformatics/multiqc-1.11:/software/singularity/3.10.3/bin:/software/bioinformatics/FastQC-0.11.7:/software/slurm-utils/bin:/software/perlbrew/0.76/perls/perl-5.36.0/bin:/software/EnvironmentModules/4.7.1/bin:/software/OSutils/git-2.21.0/bin:/software/OSutils/pandoc-1.19.2/bin:/software/OSutils/texlive-20151117/bin/x86_64-linux:/software/powerPlant/dbaas:/usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin:/opt/jupyterhub/bin:/software/perlbrew/0.76/bin:/home/cfndxa/.local/bin:/home/cfndxa/.local/bin:/home/cfndxa/.local/bin


### 3.2: Align the Reads to Reference Genome 


```bash
USER="cfndxa"
PROJECT="/workspace/$USER/MarsdenObj1/Sequencing_WGBS"
echo $PROJECT
```

    /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS



```bash
IN="/workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/002.trimmomatic"
OUT="/workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/004.alignments"
GENOME="/workspace/cfndxa/Snapper_genome/Chrysophrys_auratus.v.1.0.all.male.map.fasta"
BWA_FOLDER="/workspace/cfndxa/bwa-meth"

module load pfr-python3
module load samtools
module load bwa

# Use echo statements to be sure that the results from awk are what you really want...
FILES=`ls ${IN}/*.fastq | awk -F'[_ ]' '{print $1"_"$2"_"$3}' | sort -u`

for file in ${FILES}
    do
        NAME=`basename ${file}`
        PREFIX=`echo ${NAME} | awk -F[_] '{print $1"_"$2"_"$3"_"$4"_BWA"}'`
        file1="${file}_trimmomatic_R1.fastq"
        file2="${file}_trimmomatic_R2.fastq"

    # Align
BWA="python ${BWA_FOLDER}/bwameth.py \
    --threads 16 \
    --reference ${GENOME} \
    ${file1} ${file2} |
   samtools view -Sb -q 10 - \
   > ${OUT}/${NAME}.bam"

   echo ${BWA}
done | abatch -j ${OUT}/bwa-alignment-logs --time 10-10:01:01 --mem 20G | sbatch
```

    SBATCH_ARGS: --time 10-10:01:01 --mem 20G
    JOB_ARRAY_NAME: /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/004.alignments/bwa-alignment-logs
    GROUP_SIZE: 1
    NUM_COMMANDS: 11
    sbatch: It is not safe to run jobs over 7 days of walltime without checkpointing.
    sbatch: The time limit for this job is 10.418055555556 days.
    Submitted batch job 1063599



```bash
sbatch /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/align_ec1.sh
```

### 3.3: Sort output alignments


```bash
PROJECT="/workspace/$USER/MarsdenObj1/Sequencing_WGBS"
IN="${PROJECT}/004.alignments"
OUT="${PROJECT}/004.b.sort-alignments"
module load samtools

# Use echo statements to be sure that the results from awk are what you really want...
FILES=`ls ${IN}/*.bam`
#echo ${FILES}

for file in ${FILES}
    do
        
    NAME=`basename ${file}`
    #PREFIX=`echo ${NAME} | awk -F[_] '{print $1"_"$2"_"$3"_"$4}'`

    # Align

SORT="samtools sort ${IN}/${NAME} > ${OUT}/${NAME}"

echo ${SORT}

done | abatch -j ${OUT}/sort-alignment-logs --time 5-01:00:00 --mem 10G | sbatch
```

    SBATCH_ARGS: --time 5-01:00:00 --mem 10G
    JOB_ARRAY_NAME: /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/004.b.sort-alignments/sort-alignment-logs
    GROUP_SIZE: 1
    NUM_COMMANDS: 11
    Submitted batch job 1067172


### 3.3 Get the Statistics on the Clean BAMs


```bash
PROJECT="/workspace/$USER/MarsdenObj1/Sequencing_WGBS"
IN="${PROJECT}/004.b.sort-alignments"
OUT="${PROJECT}/004.c.stats_alignments"

module load samtools

# Use echo statements to be sure that the results from awk are what you really want...
FILES=`ls ${IN}/*.bam`
#echo ${FILES}

for file in ${FILES}
    do
        
    NAME=`basename ${file}`
    #PREFIX=`echo ${NAME} | awk -F[_] '{print $1"_"$2"_"$3"_"$4}'`

    # Align

INDEX="samtools index ${IN}/${NAME}"
            
STATS="samtools stats ${IN}/${NAME} > ${OUT}/${NAME}.txt"

COMMAND="${INDEX} | ${STATS}"
       
       echo ${COMMAND}
       
done | abatch -j ${OUT}/stats-alignment-logs --time 5-01:00:00 --mem 10G | sbatch
```

    SBATCH_ARGS: --time 5-01:00:00 --mem 10G
    JOB_ARRAY_NAME: /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/004.c.stats_alignments/stats-alignment-logs
    GROUP_SIZE: 1
    NUM_COMMANDS: 11
    Submitted batch job 1076145



```bash
sbatch /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/sort-index-stats-ec1.sh
```

    Submitted batch job 5713396


### 3.3 Get the Statistics on the Clean BAMs
#### Extract only the relevant information


```bash
PROJECT="/workspace/$USER/MarsdenObj1/Sequencing_WGBS"
IN="${PROJECT}/004.c.stats_alignments"
OUT="${PROJECT}/004.c.stats_alignments/shorter.files"

mkdir -p ${OUT}

module load samtools

# Use echo statements to be sure that the results from awk are what you really want...
FILES=`ls ${IN}/*.txt`
#echo ${FILES}

for file in ${FILES}
    do
        
    NAME=`basename ${file}`
    #PREFIX=`echo ${NAME} | awk -F[_] '{print $1"_"$2"_"$3"_"$4}'`

    # Align

CUT="grep ^SN ${IN}/${NAME} | cut -f 2- > ${OUT}/${NAME}-stats.txt"
  
       echo ${CUT}
       
done | abatch -j ${OUT}/stats-alignment-short --time 5-01:00:00 --mem 10G | sbatch
```

    SBATCH_ARGS: --time 5-01:00:00 --mem 10G
    JOB_ARRAY_NAME: /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/004.c.stats_alignments/shorter.files/stats-alignment-short
    GROUP_SIZE: 1
    NUM_COMMANDS: 11
    Submitted batch job 1076231


### 3.4 Get further statistics on the alignments using Picard tools


```bash
GENOME="/workspace/cfndxa/Snapper_genome/Chrysophrys_auratus.v.1.0.all.male.map.fasta"
PROJECT="/workspace/$USER/MarsdenObj1/Sequencing_WGBS"
IN="${PROJECT}/004.b.sort-alignments"
OUT="${PROJECT}/004.c.stats-alignments"

# Load needed modules
module load java
module load picard-tools

# Run Picard Tools to get some metrics on data & alignments
ls -1 $IN/*.bam | 
while read i
do
    file=$(basename "$i")

   ALIGNMETRICS="picard CollectAlignmentSummaryMetrics
        R=$GENOME \
        I=$IN/$file \
        O=$OUT/"$file"_alignment_metrics.txt"

  INSERTMETRICS="picard CollectInsertSizeMetrics
        I=$IN/$file \
        OUTPUT=$OUT/"$file"_insert_size_metrics.txt \
        HISTOGRAM_FILE=$OUT/"$file"_insert_size_histogram.pdf"

    #echo "Computing coverage for $file"
    #samtools depth -a "$ALIGNEDFOLDER"/"$file" | gzip - > "$METRICSFOLDER"/"$file"_coverage.gz
COMMAND="${ALIGNMETRICS} | ${INSERTMETRICS}"
       
       echo ${COMMAND}
       
done | abatch -j ${OUT}/metrics --time 5-01:00:00 --mem 10G | sbatch
```

    SBATCH_ARGS: --time 5-01:00:00 --mem 10G
    JOB_ARRAY_NAME: /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/004.c.stats-alignments/metrics
    GROUP_SIZE: 1
    NUM_COMMANDS: 11
    Submitted batch job 1076246



```bash
sbatch /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/picard_ec1.sh
```

    Submitted batch job 5715668


## 4. Remove Duplicates


```bash
PROJECT="/workspace/$USER/MarsdenObj1/Sequencing_WGBS"
IN="${PROJECT}/004.b.sort-alignments"
OUT="${PROJECT}/005.deduplication"
METRICS="${OUT}/metrics"
TMP="${OUT}/tmp"

mkdir -p $METRICS

module load java
module load picard-tools

# Use echo statements to be sure that the results from awk are what you really want...
FILES=`ls ${IN}/*.bam | awk -F'[.]' '{print $1"_"$2"_"$3}' | sort -u`

for file in ${FILES}
    do
        NAME=`basename ${file}`
         
COMMAND="picard MarkDuplicates \
        INPUT=${IN}/${NAME}.bam \
        OUTPUT=${OUT}/${NAME}.dedup.bam \
        METRICS_FILE=${METRICS}/${NAME}.txt \
        VALIDATION_STRINGENCY=SILENT \
        MAX_FILE_HANDLES=100 \
        REMOVE_DUPLICATES=true
        TMP_DIR=$TMP"          
        
    echo $COMMAND
     
done | abatch -j ${OUT}/metrics --time 5-01:00:00 --mem 10G | sbatch
```

    SBATCH_ARGS: --time 5-01:00:00 --mem 10G
    JOB_ARRAY_NAME: /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/005.deduplication/metrics
    GROUP_SIZE: 1
    NUM_COMMANDS: 11
    Submitted batch job 1118794



```bash
sbatch /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/dedup_ec1.sh
```

    Submitted batch job 5713438



```bash
sbatch /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/sortdedup_ec1.sh
```

    Submitted batch job 5715952



```bash
sbatch /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/index-dedup-ec1.sh
```

    Submitted batch job 5717863
    (/workspace/appscratch/miniconda/cfndxa_meth) 


## 5. Extract DNA methylation information
##### Prepare a python environment to install MethylDackel. Run these commands only once in previous session.


```bash
cd /workspace/cfndxa
```


```bash
bsub -I "conda create -y --name cfndxa_meth python=3"
```

    Job <900282> is submitted to default queue <lowpriority>.
    <<Waiting for dispatch ...>>
    <<Starting on aklppg32>>
    Collecting package metadata (current_repodata.json): ...working... done
    Solving environment: ...working... done
    
    
    ==> WARNING: A newer version of conda exists. <==
      current version: 4.10.3
      latest version: 4.12.0
    
    Please update conda by running
    
        $ conda update -n base -c defaults conda
    
    
    
    ## Package Plan ##
    
      environment location: /workspace/appscratch/miniconda/cfndxa_meth
    
      added / updated specs:
        - python=3
    
    
    The following packages will be downloaded:
    
        package                    |            build
        ---------------------------|-----------------
        _libgcc_mutex-0.1          |             main           3 KB
        _openmp_mutex-4.5          |            1_gnu          22 KB
        bzip2-1.0.8                |       h7b6447c_0          78 KB
        certifi-2020.6.20          |     pyhd3eb1b0_3         155 KB
        ld_impl_linux-64-2.35.1    |       h7274673_9         586 KB
        libffi-3.3                 |       he6710b0_2          50 KB
        libgcc-ng-9.3.0            |      h5101ec6_17         4.8 MB
        libgomp-9.3.0              |      h5101ec6_17         311 KB
        libstdcxx-ng-9.3.0         |      hd4cf53a_17         3.1 MB
        libuuid-1.0.3              |       h7f8727e_2          17 KB
        ncurses-6.3                |       h7f8727e_2         782 KB
        pip-21.2.4                 |  py310h06a4308_0         1.8 MB
        python-3.10.3              |       h12debd9_5        24.2 MB
        readline-8.1.2             |       h7f8727e_1         354 KB
        setuptools-58.0.4          |  py310h06a4308_0         782 KB
        sqlite-3.38.0              |       hc218d9a_0         1.0 MB
        tk-8.6.11                  |       h1ccaba5_0         3.0 MB
        tzdata-2021e               |       hda174b7_0         112 KB
        wheel-0.37.1               |     pyhd3eb1b0_0          33 KB
        xz-5.2.5                   |       h7b6447c_0         341 KB
        zlib-1.2.11                |       h7f8727e_4         108 KB
        ------------------------------------------------------------
                                               Total:        41.6 MB
    
    The following NEW packages will be INSTALLED:
    
      _libgcc_mutex      pkgs/main/linux-64::_libgcc_mutex-0.1-main
      _openmp_mutex      pkgs/main/linux-64::_openmp_mutex-4.5-1_gnu
      bzip2              pkgs/main/linux-64::bzip2-1.0.8-h7b6447c_0
      ca-certificates    pkgs/main/linux-64::ca-certificates-2022.3.18-h06a4308_0
      certifi            pkgs/main/noarch::certifi-2020.6.20-pyhd3eb1b0_3
      ld_impl_linux-64   pkgs/main/linux-64::ld_impl_linux-64-2.35.1-h7274673_9
      libffi             pkgs/main/linux-64::libffi-3.3-he6710b0_2
      libgcc-ng          pkgs/main/linux-64::libgcc-ng-9.3.0-h5101ec6_17
      libgomp            pkgs/main/linux-64::libgomp-9.3.0-h5101ec6_17
      libstdcxx-ng       pkgs/main/linux-64::libstdcxx-ng-9.3.0-hd4cf53a_17
      libuuid            pkgs/main/linux-64::libuuid-1.0.3-h7f8727e_2
      ncurses            pkgs/main/linux-64::ncurses-6.3-h7f8727e_2
      openssl            pkgs/main/linux-64::openssl-1.1.1n-h7f8727e_0
      pip                pkgs/main/linux-64::pip-21.2.4-py310h06a4308_0
      python             pkgs/main/linux-64::python-3.10.3-h12debd9_5
      readline           pkgs/main/linux-64::readline-8.1.2-h7f8727e_1
      setuptools         pkgs/main/linux-64::setuptools-58.0.4-py310h06a4308_0
      sqlite             pkgs/main/linux-64::sqlite-3.38.0-hc218d9a_0
      tk                 pkgs/main/linux-64::tk-8.6.11-h1ccaba5_0
      tzdata             pkgs/main/noarch::tzdata-2021e-hda174b7_0
      wheel              pkgs/main/noarch::wheel-0.37.1-pyhd3eb1b0_0
      xz                 pkgs/main/linux-64::xz-5.2.5-h7b6447c_0
      zlib               pkgs/main/linux-64::zlib-1.2.11-h7f8727e_4
    
    
    
    Downloading and Extracting Packages
    libgomp-9.3.0        | 311 KB    | ########## | 100% 
    libgcc-ng-9.3.0      | 4.8 MB    | ########## | 100% 
    tk-8.6.11            | 3.0 MB    | ########## | 100% 
    sqlite-3.38.0        | 1.0 MB    | ########## | 100% 
    python-3.10.3        | 24.2 MB   | ########## | 100% 
    tzdata-2021e         | 112 KB    | ########## | 100% 
    libuuid-1.0.3        | 17 KB     | ########## | 100% 
    zlib-1.2.11          | 108 KB    | ########## | 100% 
    setuptools-58.0.4    | 782 KB    | ########## | 100% 
    libstdcxx-ng-9.3.0   | 3.1 MB    | ########## | 100% 
    certifi-2020.6.20    | 155 KB    | ########## | 100% 
    _openmp_mutex-4.5    | 22 KB     | ########## | 100% 
    _libgcc_mutex-0.1    | 3 KB      | ########## | 100% 
    wheel-0.37.1         | 33 KB     | ########## | 100% 
    ncurses-6.3          | 782 KB    | ########## | 100% 
    pip-21.2.4           | 1.8 MB    | ########## | 100% 
    libffi-3.3           | 50 KB     | ########## | 100% 
    xz-5.2.5             | 341 KB    | ########## | 100% 
    readline-8.1.2       | 354 KB    | ########## | 100% 
    ld_impl_linux-64-2.3 | 586 KB    | ########## | 100% 
    bzip2-1.0.8          | 78 KB     | ########## | 100% 
    Preparing transaction: ...working... done
    Verifying transaction: ...working... done
    Executing transaction: ...working... done
    #
    # To activate this environment, use
    #
    #     $ conda activate cfndxa_meth
    #
    # To deactivate an active environment, use
    #
    #     $ conda deactivate
    



```bash
conda activate cfndxa_meth
```

    (/workspace/appscratch/miniconda/cfndxa_meth) 



```bash
conda install -y -c bioconda/label/cf201901 methyldackel 
```

    Collecting package metadata (current_repodata.json): done
    Solving environment: done
    
    
    ==> WARNING: A newer version of conda exists. <==
      current version: 4.10.3
      latest version: 4.12.0
    
    Please update conda by running
    
        $ conda update -n base -c defaults conda
    
    
    
    ## Package Plan ##
    
      environment location: /workspace/appscratch/miniconda/cfndxa_meth
    
      added / updated specs:
        - methyldackel
    
    
    The following NEW packages will be INSTALLED:
    
      methyldackel       bioconda/label/cf201901/linux-64::methyldackel-0.3.0-ha92aebf_2
    
    
    Preparing transaction: done
    Verifying transaction: done
    Executing transaction: done
    (/workspace/appscratch/miniconda/cfndxa_meth) 



This needs to be run only once


```bash
module load java
module load picard-tools
```


```bash
picard NormalizeFasta I="/workspace/cfndxa/Snapper_genome/Chrysophrys_auratus.v.1.0.all.male.map.fasta" O="/workspace/cfndxa/Snapper_genome/Chrysophrys_auratus.v.1.0.all.male.map-PicardNormalize.fasta"
```

    17:05:24.801 INFO  NativeLibraryLoader - Loading libgkl_compression.so from jar:file:/software/bioinformatics/picard-tools-2.18.7/picard.jar!/com/intel/gkl/native/libgkl_compression.so
    [Wed Mar 30 17:05:24 NZDT 2022] NormalizeFasta INPUT=/workspace/cfndxa/Snapper_genome/Chrysophrys_auratus.v.1.0.all.male.map.fasta OUTPUT=/workspace/cfndxa/Snapper_genome/Chrysophrys_auratus.v.1.0.all.male.map-PicardNormalize.fasta    LINE_LENGTH=100 TRUNCATE_SEQUENCE_NAMES_AT_WHITESPACE=false VERBOSITY=INFO QUIET=false VALIDATION_STRINGENCY=STRICT COMPRESSION_LEVEL=5 MAX_RECORDS_IN_RAM=500000 CREATE_INDEX=false CREATE_MD5_FILE=false GA4GH_CLIENT_SECRETS=client_secrets.json USE_JDK_DEFLATER=false USE_JDK_INFLATER=false
    [Wed Mar 30 17:05:24 NZDT 2022] Executing as cfndxa@aklppj31.pfr.co.nz on Linux 3.10.0-1160.45.1.el7.x86_64 amd64; OpenJDK 64-Bit Server VM 1.8.0_312-b07; Deflater: Intel; Inflater: Intel; Provider GCS is not available; Picard version: 2.18.7-SNAPSHOT
    [Wed Mar 30 17:05:45 NZDT 2022] picard.reference.NormalizeFasta done. Elapsed time: 0.35 minutes.
    Runtime.totalMemory()=1448607744


### 5.1 M-bias plot DNA methylation information

We need to run the M-bias plot before extracting DNA methylation data because it will help us determine the --OT and --OB command of the methylation extraction


```bash
PROJECT="/workspace/$USER/MarsdenObj1/Sequencing_WGBS"
IN="${PROJECT}/005.deduplication"
OUT="${PROJECT}/006.methextraction/001.methbias"
GENOME="/workspace/cfndxa/Snapper_genome/Chrysophrys_auratus.v.1.0.all.male.map-PicardNormalize.fasta"

# Modules
conda activate cfndxa_meth

### This option is good to set when using pipes...
set -o pipefail
# Use echo statements to be sure that the results from awk are what you really want...
FILES=`ls ${IN}/*.bam | awk -F'[.]' '{print $1"_"$2}' | sort -u`

for file in ${FILES}
    do
        NAME=`basename ${file}`

COMMAND="MethylDackel mbias $GENOME ${IN}/${NAME}.dedup.bam ${OUT}/${NAME}_mbias"

     echo $COMMAND
     
done | abatch -j ${OUT}/mbias --time 5-01:00:00 --mem 10G | sbatch
```

    (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) SBATCH_ARGS: --time 5-01:00:00 --mem 10G
    JOB_ARRAY_NAME: /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/006.methextraction/001.methbias/mbias
    GROUP_SIZE: 1
    NUM_COMMANDS: 11
    Submitted batch job 1154097
    (/workspace/appscratch/miniconda/cfndxa_meth) 




```bash
sbatch /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/mbias_ec1.sh
```

    Submitted batch job 5717904
    (/workspace/appscratch/miniconda/cfndxa_meth) 


### 5.1 Extract DNA methylation information for methylKit

- Only for sample no. 4= EC_4 mbias plot suggests to exlcude 4 bases: Suggested inclusion options: --OT 0,0,0,0 --OB 2,0,0,0  
- For the rest of samples: Suggested inclusion options: --OT 0,0,0,0 --OB 0,0,0,0


```bash
PROJECT="/workspace/$USER/MarsdenObj1/Sequencing_WGBS"
IN="${PROJECT}/005.deduplication"
OUT="${PROJECT}/006.methextraction"
GENOME="/workspace/cfndxa/Snapper_genome/Chrysophrys_auratus.v.1.0.all.male.map-PicardNormalize.fasta"
LOG="${OUT}/logs"

mkdir -p $OUT
mkdir -p $LOG

# Modules
conda activate cfndxa_meth

### This option is good to set when using pipes...
set -o pipefail
# Use echo statements to be sure that the results from awk are what you really want...
FILES=`ls ${IN}/*.bam | awk -F'[.]' '{print $1"_"$2}' | sort -u`

for file in ${FILES}
    do
        NAME=`basename ${file}`
   
COMMAND="MethylDackel extract --OT 0,0,0,0 --OB 0,0,0,0 -d 10 --maxVariantFrac 0.05 --mergeContext -o ${OUT}/${NAME}_mx-merged $GENOME ${IN}/${NAME}.dedup.bam"

     echo $COMMAND
     
done | abatch -j ${OUT}/methextraction --time 5-01:00:00 --mem 10G | sbatch
```

    (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) SBATCH_ARGS: --time 5-01:00:00 --mem 10G
    JOB_ARRAY_NAME: /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/006.methextraction/methextraction
    GROUP_SIZE: 1
    NUM_COMMANDS: 11
    Submitted batch job 1126132
    (/workspace/appscratch/miniconda/cfndxa_meth) 



- Run only for sample no. 4= EC_4 mbias plot suggests to exlcude 4 bases: Suggested inclusion options: --OT 0,0,0,0 --OB 2,0,0,0  


```bash
PROJECT="/workspace/$USER/MarsdenObj1/Sequencing_WGBS"
IN="${PROJECT}/005.deduplication"
OUT="${PROJECT}/006.methextraction"
GENOME="/workspace/cfndxa/Snapper_genome/Chrysophrys_auratus.v.1.0.all.male.map-PicardNormalize.fasta"
LOG="${OUT}/logs"

mkdir -p $OUT
mkdir -p $LOG

# Modules
conda activate cfndxa_meth

### This option is good to set when using pipes...
set -o pipefail
# Use echo statements to be sure that the results from awk are what you really want...
FILES=`ls ${IN}/*.bam | awk -F'[.]' '{print $1"_"$2}' | sort -u`

for file in ${FILES}
    do
        NAME=`basename ${file}`
   
COMMAND="MethylDackel extract --OT 0,0,0,0 --OB 2,0,0,0 -d 10 --maxVariantFrac 0.05 --mergeContext -o ${OUT}/${NAME}_mx-merged $GENOME ${IN}/${NAME}.dedup.bam"

     echo $COMMAND
     
done | abatch -j ${OUT}/methextraction --time 5-01:00:00 --mem 10G | sbatch
```

    (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) (/workspace/appscratch/miniconda/cfndxa_meth) SBATCH_ARGS: --time 5-01:00:00 --mem 10G
    JOB_ARRAY_NAME: /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/006.methextraction/methextraction
    GROUP_SIZE: 1
    NUM_COMMANDS: 11
    Submitted batch job 1126132
    (/workspace/appscratch/miniconda/cfndxa_meth) 




```bash
sbatch /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/methextract_ec1.sh
```

    Submitted batch job 5718736
    (/workspace/appscratch/miniconda/cfndxa_meth) 



```bash
head -100 /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/methextract_ec1.sh
```

    #!/bin/bash
    #SBATCH -J "ec1-methextract"
    #SBATCH -o log_%j
    #SBATCH -c 4 
    #SBATCH -p medium
    #SBATCH --time=5-00:00
    #SBATCH --mem=20G
    
    # Modules
    conda activate cfndxa_meth
    
    MethylDackel extract --OT 0,0,0,0 --OB 0,0,0,0 -d 10 --maxVariantFrac 0.05 --mergeContext -o /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/006.methextraction/EC_1_mx-merged /workspace/cfndxa/Snapper_genome/Chrysophrys_auratus.v.1.0.all.male.map-PicardNormalize.fasta /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/005.deduplication/EC_1.dedup.bam



```bash
MethylDackel extract
```

    
    Usage: MethylDackel extract [OPTIONS] <ref.fa> <sorted_alignments.bam>
    
    Options:
     -q INT           Minimum MAPQ threshold to include an alignment (default 10)
     -p INT           Minimum Phred threshold to include a base (default 5). This
                      must be >0.
     -D INT           Maximum per-base depth (default 2000)
     -d INT           Minimum per-base depth for reporting output. If you use
                      --mergeContext, this then applies to the merged CpG/CHG.
                      (default 1)
     -r STR           Region string in which to extract methylation
     -l FILE          A BED file listing regions for inclusion.
     --keepStrand     If a BED file is specified, then this option will cause the
                      strand column (column 6) to be utilized, if present. Thus, if
                      a region has a '+' in this column, then only metrics from the
                      top strand will be output. Note that the -r option can be used
                      to limit the regions of -l.
     -@ nThreads      The number of threads to use, the default 1
     --chunkSize INT  The size of the genome processed by a single thread at a time.
                      The default is 1000000 bases. This value MUST be at least 1.
     --mergeContext   Merge per-Cytosine metrics from CpG and CHG contexts into
                      per-CPG or per-CHG metrics.
     -o, --opref STR  Output filename prefix. CpG/CHG/CHH context metrics will be
                      output to STR_CpG.bedGraph and so on.
     --keepDupes      By default, any alignment marked as a duplicate is ignored.
                      This option causes them to be incorporated.
     --keepSingleton  By default, if only one read in a pair aligns (a singleton)
                      then it's ignored.
     --keepDiscordant By default, paired-end alignments with the properly-paired bit
                      unset in the FLAG field are ignored. Note that the definition
                      of concordant and discordant is based on your aligner
                      settings.
     -F, --ignoreFlags    By deault, any alignment marked as secondary (bit 0x100),
                      failing QC (bit 0x200), a PCR/optical duplicate (0x400) or
                      supplemental (0x800) is ignored. This equates to a value of
                      0xF00 or 3840 in decimal. If you would like to change that,
                      you can specify a new value here.
                      ignored. Specifying this causes them to be included.
     -R, --requireFlags   Require each alignment to have all bits in this value
                      present, or else the alignment is ignored. This is equivalent
                      to the -f option in samtools. The default is 0, which
                      includes all alignments.
     --noCpG          Do not output CpG context methylation metrics
     --CHG            Output CHG context methylation metrics
     --CHH            Output CHH context methylation metrics
     --fraction       Extract fractional methylation (only) at each position. This
                      produces a file with a .meth.bedGraph extension.
     --counts         Extract base counts (only) at each position. This produces a
                      file with a .counts.bedGraph extension.
     --logit          Extract logit(M/(M+U)) (only) at each position. This produces
                      a file with a .logit.bedGraph extension.
     --minOppositeDepth   If you would like to exclude sites that likely contain
                      SNPs, then specifying a value greater than 0 here will
                      indicate the minimum depth required on the strand opposite of
                      a C to look for A/T/C bases. The fraction of these necessary
                      to exclude a position from methylation extraction is specified
                      by the --maxVariantFrac parameter. The default is 0, which
                      means that no positions will be excluded. Note that the -p and
                      -q apply here as well. Note further that if you use
                      --mergeContext that a merged site will be excluded if either
                      of its individual Cs would be excluded.
     --maxVariantFrac The maximum fraction of A/T/C base calls on the strand
                      opposite of a C to allow before a position is declared a
                      variant (thereby being excluded from output). The default is
                      0.0. See also --minOppositeDepth.
     --methylKit      Output in the format required by methylKit. Note that this is
                      incompatible with --mergeContext, --fraction and --counts.
     --OT INT,INT,INT,INT Inclusion bounds for methylation calls from reads/pairs
                      originating from the original top strand. Suggested values can
                      be obtained from the MBias program. Each integer represents a
                      1-based position on a read. For example --OT A,B,C,D
                      translates to, "Include calls at positions from A through B
                      on read #1 and C through D on read #2". If a 0 is used a any
                      position then that is translated to mean start/end of the
                      alignment, as appropriate. For example, --OT 5,0,0,0 would
                      include all but the first 4 bases on read #1. Users are
                      strongly advised to consult a methylation bias plot, for
                      example by using the MBias program.
     --OB INT,INT,INT,INT
     --CTOT INT,INT,INT,INT
     --CTOB INT,INT,INT,INT As with --OT, but for the original bottom, complementary
                      to the original top, and complementary to the original bottom
                      strands, respectively.
     --nOT INT,INT,INT,INT Like --OT, but always exclude INT bases from a given end
                      from inclusion,regardless of the length of an alignment. This
                      is useful in cases where reads may have already been trimmed
                      to different lengths, but still none-the-less contain a
                      certain length bias at one or more ends.
     --nOB INT,INT,INT,INT
     --nCTOT INT,INT,INT,INT
     --nCTOB INT,INT,INT,INT As with --nOT, but for the original bottom, complementary
                      to the original top, and complementary to the original bottom
                      strands, respectively.
     --version        Print version and then quit.
    
    Note that --fraction, --counts, and --logit are mutually exclusive!
    (/workspace/appscratch/miniconda/cfndxa_meth) 



```bash
conda deactivate
```


```bash
head -10 006.methextraction/EC_1_mx-merged_CpG.bedGraph
```

    track type="bedGraph" description="/workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/006.methextraction/EC_1_mx-merged CpG merged methylation levels"
    LG1	417	419	75	9	3
    LG1	447	449	88	16	2
    LG1	465	467	78	15	4
    LG1	512	514	77	21	6
    LG1	608	610	82	32	7
    LG1	862	864	72	27	10
    LG1	1018	1020	80	21	5
    LG1	1046	1048	88	22	3
    LG1	1080	1082	91	22	2



```bash
gunzip 006.methextraction/*mx-merged_CpG.bedGraph.gz
```

### 5.2 Convert DNA methylation values files to DSS compatible


```bash
ls
```

    000.raw				 log_1887613  log_2074060
    001.fastqc_raw			 log_1887813  log_2074061
    001.fastq_raw_merged		 log_1901836  log_5713105
    002.trimmomatic			 log_1901838  log_5713396
    003.fastq_trimmomatic		 log_1901840  log_5713437
    004.alignments			 log_1940687  log_5713438
    004.b.sort-alignments		 log_1947680  log_5715668
    004.c.stats_alignments		 log_1947683  log_5715952
    005.b.sort-deduplication	 log_1952030  log_5717843
    005.deduplication		 log_1952032  log_5717863
    006.methextraction		 log_1982768  log_5717904
    007.methylkit			 log_1985622  log_5718098
    008.methylation-analysis	 log_2002416  log_5718434
    099.test			 log_2002417  log_5718736
    align_ec1.sh			 log_2005282  mbias_ec1.sh
    dedup_ec1.sh			 log_2005303  methextract_ec1.sh
    index-dedup-ec1.sh		 log_2005317  picard_ec1.sh
    Install_DSS_devel_version.ipynb  log_2007671  Sequencing_WGBS.Rproj
    log_1731997			 log_2007673  sortdedup_ec1.sh
    log_1741614			 log_2007679  sort-index-stats-ec1.sh
    log_1741858			 log_2007680  Untitled.ipynb
    log_1741912			 log_2007695  WGBS-Obj1-MethylKit.ipynb
    log_1741923			 log_2066306  WGBS-Obj1-WildFish-Marsden.ipynb
    log_1742109			 log_2072104  WGBS-statistics.xlsx
    log_1759681			 log_2072343
    log_1759749			 log_2072350



```bash
cd 006.methextraction
ls
```

     001.dss		      'methylDB 2023-04-19 7ki'
     001.methbias		      'methylDB 2023-04-19 pq1'
     EC_1_mx-merged_CpG.bedGraph  'methylDB 2023-06-23 JH4'
     EC_2_mx-merged_CpG.bedGraph  'methylDB 2023-06-26 b1z'
     EC_3_mx-merged_CpG.bedGraph   samples.txt
     EC_4_mx-merged_CpG.bedGraph   subset_10000
     EC_5_mx-merged_CpG.bedGraph   WC_1_mx-merged_CpG.bedGraph
     EC_6_mx-merged_CpG.bedGraph   WC_2_mx-merged_CpG.bedGraph
     extraction_conversion.sh      WC_3_mx-merged_CpG.bedGraph
     methextraction		       WC_5_mx-merged_CpG.bedGraph
     methextraction-ec4	       WC_6_mx-merged_CpG.bedGraph



```bash
find . -name "*_mx-merged_CpG.bedGraph" | xargs -n 1 bash extraction_conversion.sh
```


```bash
head 006.methextraction/extraction_conversion.sh
```

    #!/bin/bash
    set -e
    set -u
    set -o pipefail
    
    sample_name=$(basename -s "_mx-merged_CpG.bedGraph" "$1")
    awk '{if (NR>1) {print $1, $2, $3=$5+$6, $5}}' ${sample_name}_mx-merged_CpG.bedGraph \
    | awk 'BEGIN{print "chr	pos	N	X"}1' \
    | awk 'BEGIN{OFS ="\t"}{print $1, $2, $3, $4}' > 001.dss/${sample_name}-DSS.txt



```bash
wc -l EC_1_CpG.methylKit_CpG.methylKit.gz
```

    886498 EC_1_CpG.methylKit_CpG.methylKit.gz



```bash
wc -l EC_1_mx-merged_CpG.bedGraph
```

    11992563 EC_1_mx-merged_CpG.bedGraph



```bash
head 006.methextraction/001.dss/EC_1-DSS.txt
```

    chr	pos	N	X
    LG1	447	14	12
    LG1	465	15	13
    LG1	512	21	17
    LG1	608	30	23
    LG1	862	29	22
    LG1	1018	21	18
    LG1	1046	20	19
    LG1	1080	19	17
    LG1	1083	18	15



```bash
cd 008.methylation-analysis
ls
```

     02_Global_methylation_PCA.R
     Annotation_GeneFeatures.R
     anova-all-5var.Rdata
     anova-all.Rdata
     anova-axis-5var.Rdata
     anova-axis.Rdata
     anova-term-5var.Rdata
     anova-term.Rdata
     Bray-Curtis_methylation_distnaces.tiff
     combined_results_all_dmcs_groups.Rdata
     combined_results_all_dmcs_groups-unitedCpGs.Rdata
     combined_results_all_dmcs.Rdata.gz
     combined_results_dmcs.Rdata
     combined_results.Rdata
     Correlation_analysis_distances.R
     Correlation_meth-env_distance.tiff
     Correlation_meth-env-gen_distance.tiff
     Correlation_meth-env-geo_distance-Kendall.tiff
     Correlation-samples.tiff
     CpG_association.R
     Differential_methylation-DSS.R
     Distribution-Gene-features-R35.ipynb
     DMLfit-stock-wildsnapper.Rdata
     dmlTest.EC1-EC2.Rdata
     DMLtest-stock-wildsnapper.Rdata
     DMR-stock-wildsnapper.Rdata
     DSSobj-wildsnapper.Rdata
     DSSobj-wildsnapper-unitedCpGs.Rdata
     Environmental-association-analysis.R
    'Gao MEC Dataset_code'
     GlobalMethylation-perArea.tiff
     GlobalMethylation.R
     kpca.R
     kpca.sh
     lfmm_ridge_cv.R
     lfmm_ridge_cv.sh
     log_5718948
     Methylation_gene_features.R
     methylation-PCA-allCpGs.tiff
     methylation_per_area.Rdata
     MethylKit_files_reading.R
     MethylKit_files_reading.sh
     number_polymorphic_pairwise_CpGs.xlsx
     pairwise_all_combined_results_all_dmcs.Rdata
     pairwise-All-DMC-DSS-parallel-su.r
     pairwise-all-dss-su.sh
     pairwise-DMC-DSS-parallel-su.r
     Pairwise-DSS-ec12.r
     pairwise-DSS-parallel.r
     pairwise-DSS-parallel-su.r
     Pairwise-DSS.r
     Pairwise-DSS-results.R
     pairwise-dss.sh
     pairwise-dss-su.sh
     pairwise-groups-DMCs-DSS-parallel.r
     perc-meth-all.Rdata
     perc-meth-canchr.Rdata
     PhiST-np.R
     PhiST.R
     phist.sh
     Polymorphic-DMCs-Genome-wide-Obj1.ipynb
     Polymorphic_DMCs_methylation-pairwisepops.txt
     Polymorphic_DMCs_methylationpops.Rdata
     Polymorphic_DMCs_methylationpops-rowsindividuals.Rdata
     Polymorphic_DMCs_methylation.Rdata
     Polymorphic_DMCs_methylation.txt
     Polymorphic_DMCs-pairwise.Rdata
     Polymorphic_DMCs.Rdata
     Polymorphic_DMCs.txt
     populations-DMC-DSS-parallel-su.r
     populations-dss-su.sh
     Principal_components_PCi.Rdata
     rda-3vars.sh
     RDA-ANOVA-5vars.R
     RDA-ANOVA.R
     rda.meth.Rdata
     RDA-methylation-Envinromental_variables_correlations.R
     RDA-methylation-Envinromental_variables_correlations_update.R
     RDA-methylation.R
     rda.sh
     RDA.tiff
     Results-R-enrichment_methylation_gene_featurse.txt
     RSam-DSSobj-wildsnapper.Rdata
     samples_coasts.txt
     slurm-1759749.Rout
     slurm-1887613.Rout
     slurm-1887813.Rout
     slurm-1901836.Rout
     slurm-1901838.Rout
     slurm-1901840.Rout
     slurm-1940687.Rout
     slurm-1947680.Rout
     slurm-1947683.Rout
     slurm-1952032.Rout
     slurm-2005317.Rout
     slurm-2066306.Rout
     slurm-2072343.Rout
     slurm-2072350.Rout
     slurm-2074060.Rout
     slurm-2074061.Rout
     slurm-5718948.Rout
     Thumbs.db
     WGBS-Obj1-DiffMeth.ipynb



```bash
sbatch /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/008.methylation-analysis/MethylKit_files_reading.sh
```

    Submitted batch job 5718948



```bash
cd methylDB_2024-06-14_e3D
ls
```

    ec1.txt		 ec2.txt.bgz	  ec3.txt.bgz.tbi  ec5.txt
    ec1.txt.bgz	 ec2.txt.bgz.tbi  ec4.txt	   ec5.txt.bgz
    ec1.txt.bgz.tbi  ec3.txt	  ec4.txt.bgz	   ec5.txt.bgz.tbi
    ec2.txt		 ec3.txt.bgz	  ec4.txt.bgz.tbi  ec6.txt



```bash
head -20 ec1.txt
```

    #Date:2024-06-14 10:04:05
    #Class:methylRawDB
    #DT:tabix
    #SI:ec1
    #AS:snapper
    #CT:CpG
    #RS:base
    #NR:12197179
    #DT:tabix
    CauratusV1_scaffold_1002	147	149	*	26	14	12
    CauratusV1_scaffold_1002	368	370	*	39	15	24
    CauratusV1_scaffold_1002	420	422	*	49	31	18
    CauratusV1_scaffold_1002	423	425	*	53	47	6
    CauratusV1_scaffold_1002	1059	1061	*	21	9	12
    CauratusV1_scaffold_1002	1123	1125	*	16	9	7
    CauratusV1_scaffold_1002	1201	1203	*	11	9	2
    CauratusV1_scaffold_1002	3389	3391	*	12	6	6
    CauratusV1_scaffold_1002	3392	3394	*	12	8	4
    CauratusV1_scaffold_1002	3490	3492	*	53	22	31
    CauratusV1_scaffold_1002	3672	3674	*	87	45	42


## 6. Run pairwise DSS analysis

Be careful with the version of DSS used because there has been an issue with parallel computing in previous versions: https://github.com/haowulab/DSS/issues/23


```bash
module load R
```

    Loading [1mR/4.0.0[22m
      [94mLoading requirement[0m: unixODBC/2.3.0 JAGS/4.2.0 gdal/2.4.0 proj/5.2.0



```bash
Rscript /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/008.methylation-analysis/Pairwise-DSS.r
```

    Loading required package: Biobase
    Loading required package: BiocGenerics
    Loading required package: parallel
    
    Attaching package: 'BiocGenerics'
    
    The following objects are masked from 'package:parallel':
    
        clusterApply, clusterApplyLB, clusterCall, clusterEvalQ,
        clusterExport, clusterMap, parApply, parCapply, parLapply,
        parLapplyLB, parRapply, parSapply, parSapplyLB
    
    The following objects are masked from 'package:stats':
    
        IQR, mad, sd, var, xtabs
    
    The following objects are masked from 'package:base':
    
        anyDuplicated, append, as.data.frame, basename, cbind, colnames,
        dirname, do.call, duplicated, eval, evalq, Filter, Find, get, grep,
        grepl, intersect, is.unsorted, lapply, Map, mapply, match, mget,
        order, paste, pmax, pmax.int, pmin, pmin.int, Position, rank,
        rbind, Reduce, rownames, sapply, setdiff, sort, table, tapply,
        union, unique, unsplit, which.max, which.min
    
    Welcome to Bioconductor
    
        Vignettes contain introductory material; view with
        'browseVignettes()'. To cite Bioconductor, see
        'citation("Biobase")', and for packages 'citation("pkgname")'.
    
    Loading required package: BiocParallel
    Loading required package: bsseq
    Loading required package: GenomicRanges
    Loading required package: stats4
    Loading required package: S4Vectors
    
    Attaching package: 'S4Vectors'
    
    The following object is masked from 'package:base':
    
        expand.grid
    
    Loading required package: IRanges
    Loading required package: GenomeInfoDb
    Loading required package: SummarizedExperiment
    Loading required package: MatrixGenerics
    Loading required package: matrixStats
    
    Attaching package: 'matrixStats'
    
    The following objects are masked from 'package:Biobase':
    
        anyMissing, rowMedians
    
    
    Attaching package: 'MatrixGenerics'
    
    The following objects are masked from 'package:matrixStats':
    
        colAlls, colAnyNAs, colAnys, colAvgsPerRowSet, colCollapse,
        colCounts, colCummaxs, colCummins, colCumprods, colCumsums,
        colDiffs, colIQRDiffs, colIQRs, colLogSumExps, colMadDiffs,
        colMads, colMaxs, colMeans2, colMedians, colMins, colOrderStats,
        colProds, colQuantiles, colRanges, colRanks, colSdDiffs, colSds,
        colSums2, colTabulates, colVarDiffs, colVars, colWeightedMads,
        colWeightedMeans, colWeightedMedians, colWeightedSds,
        colWeightedVars, rowAlls, rowAnyNAs, rowAnys, rowAvgsPerColSet,
        rowCollapse, rowCounts, rowCummaxs, rowCummins, rowCumprods,
        rowCumsums, rowDiffs, rowIQRDiffs, rowIQRs, rowLogSumExps,
        rowMadDiffs, rowMads, rowMaxs, rowMeans2, rowMedians, rowMins,
        rowOrderStats, rowProds, rowQuantiles, rowRanges, rowRanks,
        rowSdDiffs, rowSds, rowSums2, rowTabulates, rowVarDiffs, rowVars,
        rowWeightedMads, rowWeightedMeans, rowWeightedMedians,
        rowWeightedSds, rowWeightedVars
    
    The following object is masked from 'package:Biobase':
    
        rowMedians
    
    
    Execution halted



```bash
sbatch /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/008.methylation-analysis/pairwise-dss.sh
```

    Submitted batch job 1741614



```bash
sbatch /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/008.methylation-analysis/pairwise-dss-su.sh
```

    Submitted batch job 1887813



```bash
sbatch /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/008.methylation-analysis/populations-dss-su.sh
```

    Submitted batch job 1947683


### New run with the correct trimmed file (June 2024)


```bash
sbatch /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/008.methylation-analysis/pairwise-all-dss-su.sh
```

    Submitted batch job 5726417
    (/workspace/appscratch/miniconda/cfndxa_meth) 



```bash
head -50 /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/008.methylation-analysis/pairwise-all-dss-su.sh
```

    #!/bin/bash
    #SBATCH -J "pairwise-dss"
    #SBATCH -o log_%j
    #SBATCH -c 10 
    #SBATCH -p medium
    #SBATCH --time=3-00:00
    #SBATCH --mem=20G
    
    DSS="/workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/008.methylation-analysis"
    
    cd "$DSS"
    
    #module purge
    module load R
    
    Rscript --vanilla --verbose /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/008.methylation-analysis/pairwise-All-DMC-DSS-parallel-su.r > slurm-${SLURM_JOBID}.Rout 2>&1 



```bash
head -50 /workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/008.methylation-analysis/pairwise-All-DMC-DSS-parallel-su.r
```

    # Load the required libraries
    library(DSS)
    library(parallel)
    library(dplyr)
    
    # ... (Rest of your code)
    
    # Load the object, if required
    load("/powerplant/workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/008.methylation-analysis/DSSobj-unitedCpGs-canchr.Rdata")
    
    nCPUs=10
    
    # Create the function for pairwise comparison and DMR calling
    pairwise_dml_and_dmrs <- function(groups) {
      group1 <- groups[1]
      group2 <- groups[2]
      dmlTest <- DMLtest(BSobj.united, group1 = group1, group2 = group2, smoothing = TRUE, nCPUs)
      sigdmc <- dmlTest %>% dplyr::filter(dmlTest$fdr<0.1)
      #file_name_dmlTest <- paste("/powerplant/workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/008.methylation-analysis/dmlTest.", group1, "-", group2, ".Rdata", sep = "")
      #save(dmlTest, file = file_name_dmlTest)
      #DMRs <- callDMR(dmlTest, p.threshold=0.05)
      #file_name_DMRs <- paste("/powerplant/workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/008.methylation-analysis/DMRs.", group1, "-", group2, ".Rdata", sep = "")
      #save(DMRs, file = file_name_DMRs)
      return(list(group1 = group1, group2 = group2, DMCs = dmlTest))
    }
    
    # List of group combinations for pairwise comparisons
    group_combinations <- combn(c("a", "b", "c", "d", "e", "f","g", "h", "i", "j", "k"), 2)
    
    # Perform parallel computation using DMLtest
    results <- lapply(1:ncol(group_combinations), function(i) {
      pairwise_dml_and_dmrs(group_combinations[, i])
    })
    
    # Optionally, combine the individual results into a single object
    combined_results_dmcs <- do.call(rbind, results)
    
    # Save the combined results to a file
    save(combined_results_dmcs, file = "/powerplant/workspace/cfndxa/MarsdenObj1/Sequencing_WGBS/008.methylation-analysis/pairwise_all_dmcs-canchr_correcttrimming.Rdata")



```bash
squeue -u cfndxa
```

                 JOBID PARTITION     NAME     USER ST       TIME  NODES NODELIST(REASON)


## 7.Gtf to bed


```bash
find . -type f -name '*.bam' -exec gzip "{}" \;
```


```bash
module load bedops
```

    ** INFO ** : singularity has been deprecated - please use apptainer in place.
    
    Loading [1mbedops/2.4.39[22m
      [94mLoading requirement[0m: singularity/3.10.3



```bash
pip install bedparse
```

    Defaulting to user installation because normal site-packages is not writeable
    Collecting bedparse
      Downloading bedparse-0.2.3-py3-none-any.whl (21 kB)
    Collecting argparse
      Downloading argparse-1.4.0-py2.py3-none-any.whl (23 kB)
    Requirement already satisfied: setuptools in /software/programming/miniconda3_23.1.0/lib/python3.10/site-packages (from bedparse) (65.6.3)
    Installing collected packages: argparse, bedparse
    [33m  WARNING: The script bedparse is installed in '/home/cfndxa/.local/bin' which is not on PATH.
      Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.[0m[33m
    [0mSuccessfully installed argparse-1.4.0 bedparse-0.2.3



```bash
/home/cfndxa/.local/bin/bedparse gtf2bed /workspace/cfndxa/Snapper_genome/Genome_Annotation/Chrysophrys_auratus.v.1.0.all.male.map.phase.corrected.gmap.filtered.gff3
```

    Traceback (most recent call last):
      File "/home/cfndxa/.local/bin/bedparse", line 8, in <module>
        sys.exit(main())
      File "/home/cfndxa/.local/lib/python3.10/site-packages/bedparse/bedparse.py", line 250, in main
        args.func(args)
      File "/home/cfndxa/.local/lib/python3.10/site-packages/bedparse/bedparse.py", line 225, in <lambda>
        parser_gtf2bed.set_defaults(func=lambda args: gtf2bed(args.gtf, extra=args.extraFields.split(','), filterKey=args.filterKey, filterType=args.filterType.split(','), transcript_feature_name=args.transcript_feature_name))
      File "/home/cfndxa/.local/lib/python3.10/site-packages/bedparse/converters.py", line 44, in gtf2bed
        if(line[6]!=transcripts[txName][5]):
    KeyError: 'ID=TRINITY_DN14690_c1_g1_i1.mrna1.cds.2;Name=TRINITY_DN14690_c1_g1_i1;Parent=TRINITY_DN14690_c1_g1_i1.mrna1'





```bash
/home/cfndxa/.local/bin/bedparse gtf2bed /workspace/cfndxa/Snapper_genome/Genome_Annotation/Cauratusv.1.0_annotation.combined.gtf > /workspace/cfndxa/Snapper_genome/Genome_Annotation/Cauratusv.1.0_annotation.combined.bed
```


```bash
/home/cfndxa/.local/bin/bedparse gtf2bed -h
```

    usage: bedparse gtf2bed [-h] [--extraFields EXTRAFIELDS]
                            [--filterKey FILTERKEY] [--filterType FILTERTYPE]
                            [--transcript_feature_name TRANSCRIPT_FEATURE_NAME]
                            [gtf]
    
    Converts a GTF file to BED12 format. This tool supports the Ensembl GTF
    format, which uses features of type 'transcript' (field 3) to define
    transcripts. In case the GTF file defines transcripts with a different feature
    type, it is possible to provide the feature name from the command line. If the
    GTF file also annotates 'CDS' 'start_codon' or 'stop_codon' these are used to
    annotate the thickStart and thickEnd in the BED file.
    
    positional arguments:
      gtf                   Path to the GTF file.
    
    options:
      -h, --help            show this help message and exit
      --extraFields EXTRAFIELDS
                            Comma separated list of extra GTF fields to be added
                            after col 12 (e.g. gene_id,gene_name).
      --filterKey FILTERKEY
                            GTF extra field on which to apply the filtering
      --filterType FILTERTYPE
                            Comma separated list of filterKey field values to
                            retain.
      --transcript_feature_name TRANSCRIPT_FEATURE_NAME
                            Transcript feature name. Features with this string in
                            field 3 of the GTF file will be considered
                            transcripts. (default 'transcript')



```bash
head /workspace/cfndxa/Snapper_genome/Genome_Annotation/Cauratusv.1.0_annotation.combined.gtf
```

    CauratusV1_scaffold_1002	indexed_genome	transcript	33704	33753	.	+	.	transcript_id "TCONS_00000001"; gene_id "XLOC_000001"; oId "TRINITY_DN75364_c0_g1_i1.mrna1"; tss_id "TSS1"; num_samples "2";
    CauratusV1_scaffold_1002	indexed_genome	exon	33704	33753	.	+	.	transcript_id "TCONS_00000001"; gene_id "XLOC_000001"; exon_number "1";
    CauratusV1_scaffold_1002	indexed_genome	transcript	3311	3811	.	-	.	transcript_id "TCONS_00000002"; gene_id "XLOC_000002"; oId "TRINITY_DN67007_c0_g1_i2.mrna1"; tss_id "TSS2"; num_samples "2";
    CauratusV1_scaffold_1002	indexed_genome	exon	3311	3596	.	-	.	transcript_id "TCONS_00000002"; gene_id "XLOC_000002"; exon_number "1";
    CauratusV1_scaffold_1002	indexed_genome	exon	3705	3811	.	-	.	transcript_id "TCONS_00000002"; gene_id "XLOC_000002"; exon_number "2";
    CauratusV1_scaffold_1002	indexed_genome	transcript	26967	27370	.	-	.	transcript_id "TCONS_00000003"; gene_id "XLOC_000003"; oId "TRINITY_DN14690_c1_g1_i1.mrna1"; tss_id "TSS3"; num_samples "2";
    CauratusV1_scaffold_1002	indexed_genome	exon	26967	27123	.	-	.	transcript_id "TCONS_00000003"; gene_id "XLOC_000003"; exon_number "1";
    CauratusV1_scaffold_1002	indexed_genome	exon	27265	27370	.	-	.	transcript_id "TCONS_00000003"; gene_id "XLOC_000003"; exon_number "2";
    CauratusV1_scaffold_1002	indexed_genome	transcript	30282	34901	.	-	.	transcript_id "TCONS_00000004"; gene_id "XLOC_000004"; oId "TRINITY_DN86978_c2_g1_i4.mrna1"; tss_id "TSS4"; num_samples "2";
    CauratusV1_scaffold_1002	indexed_genome	exon	30282	30975	.	-	.	transcript_id "TCONS_00000004"; gene_id "XLOC_000004"; exon_number "1";



```bash
head /workspace/cfndxa/Snapper_genome/Genome_Annotation/Chrysophrys_auratus.v.1.0.all.male.map.phase.corrected.gmap.filtered.gff3
```

    ##gff-version 3
    ##sequence-region CauratusV1_scaffold_1002 1 52396
    CauratusV1_scaffold_1002	indexed_genome	gene	26967	27370	.	-	.	ID=TRINITY_DN14690_c1_g1_i1.path1;Name=TRINITY_DN14690_c1_g1_i1
    CauratusV1_scaffold_1002	indexed_genome	mRNA	26967	27370	.	-	.	ID=TRINITY_DN14690_c1_g1_i1.mrna1;Name=TRINITY_DN14690_c1_g1_i1;Parent=TRINITY_DN14690_c1_g1_i1.path1;coverage=84.0;identity=93.2;indels=0;matches=245;mismatches=18;unknowns=0
    CauratusV1_scaffold_1002	indexed_genome	CDS	26969	27123	89	-	2	ID=TRINITY_DN14690_c1_g1_i1.mrna1.cds.2;Name=TRINITY_DN14690_c1_g1_i1;Parent=TRINITY_DN14690_c1_g1_i1.mrna1
    CauratusV1_scaffold_1002	indexed_genome	CDS	27265	27370	98	-	0	ID=TRINITY_DN14690_c1_g1_i1.mrna1.cds.1;Name=TRINITY_DN14690_c1_g1_i1;Parent=TRINITY_DN14690_c1_g1_i1.mrna1
    CauratusV1_scaffold_1002	indexed_genome	exon	26967	27123	89	-	.	ID=TRINITY_DN14690_c1_g1_i1.mrna1.exon2;Name=TRINITY_DN14690_c1_g1_i1;Parent=TRINITY_DN14690_c1_g1_i1.mrna1
    CauratusV1_scaffold_1002	indexed_genome	exon	27265	27370	98	-	.	ID=TRINITY_DN14690_c1_g1_i1.mrna1.exon1;Name=TRINITY_DN14690_c1_g1_i1;Parent=TRINITY_DN14690_c1_g1_i1.mrna1
    ###
    CauratusV1_scaffold_1002	indexed_genome	gene	46803	48192	.	-	.	ID=TRINITY_DN27126_c0_g1_i1.path1;Name=TRINITY_DN27126_c0_g1_i1


## RUN UP TO HERE
