# ChloroBras!

![Alt text](https://user-images.githubusercontent.com/108393526/176390402-1a60a2dc-f4c4-48db-a3b0-d87b2c1a3f24.png)


## Parameters

Defines the pipeline inputs parameters
Each of the following parameters can be specified as command line options or in the config file
Beware of quotes when necessary and do not forget to modify the path when necessary


### Test_assembler

   Reads directory
    --readsFiles                    Path to input data, default: "./samples/*_R{1,2}.fastq.gz"

    Results directory
    --resultsDir                    Path to results directory, default: "./results/"

    Sqtk
    --seqtk_nb_read                 Number of reads to keep, default: 2000000

    GetOrganelle
    --getorganelle_index            Index of GetOrganelle, default: "embplant_pt"
    --getorganelle_kmer             Size of kmers, default: "21,45,65,85,105"

    FastPlast
    --fastplast_index               Index of Fast-Plast, default: "Brassicales"

    OrgAsm
    --orgasm_probes                 Index of ORGanelle ASeMbler, default: "protChloroArabidopsis"

    Rename_headers
    --rename_dir_script             Absolute path to script rename

    Nucmer
    --nucmer_ref                    Absolute path to Fasta reference for alignment, default: brassica oleracea

    Mummer
    --mummer_axe                    Size of X-axis (fonction of genome's size), default (plastome): "'[0:154000]'"
    --mummer_format_output          Format of the plot, default: "png"

### Analysis_chloro

    Reads directory
    --readsFiles                    Path to input data, default: "./samples/*_R{1,2}.fastq.gz"

    Results directory
    --resultsDir                    Path to results directory, default: "./results/"

    GetOrganelle
    --getorganelle_index            Index of GetOrganelle, default: "embplant_pt"
    --getorganelle_kmer             Size of kmers, default: "21,45,65,85,105"

    Rename_headers
    --rename_dir_script             Absolute path to script rename

    Nucmer
    --nucmer_ref                    Absolute path to Fasta reference for alignment, default: brassica oleracea

    Mummer
    --mummer_axe                    Size of X-axis (fonction of genome's size), default (plastome): "'[0:154000]'"
    --mummer_format_output          Format of the plot, default: "png"

    Select_assembly
    --select_assembly_script        Absolute path to script select_assembly

    Mafft
    --mafft_method                  Alignment methods, default: "auto"

    Rename_headers_phylo
    --rename_headers_phylo_script   Absolute path to script rename

    Raxml
    --raxml_model                   Model uses by RAxML, default: "GTRGAMMAI"
    
