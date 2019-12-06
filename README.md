# utl-meta-analysis-of-deaths-in-twenty-studies-with-forest-plot
Meta analysis of deaths in twenty studies with forest plot
    Meta analysis of deaths in twenty studies with forest plot                                                                           
                                                                                                                                         
    Probablility of Death based on 23 studies in four countries(fixed effect)                                                            
                                                                                                                                         
    Ficticious data                                                                                                                      
                                                                                                                                         
    For forest plot see                                                                                                                  
    https://tinyurl.com/s6embs9                                                                                                          
    https://github.com/rogerjdeangelis/utl-meta-analysis-of-deaths-in-twenty-studies-with-forest-plot/blob/master/forest.pdf             
                                                                                                                                         
    github                                                                                                                               
    https://tinyurl.com/vb5jbub                                                                                                          
    https://github.com/rogerjdeangelis/utl-meta-analysis-of-deaths-in-twenty-studies-with-forest-plot                                    
                                                                                                                                         
    SAS Forum                                                                                                                            
    https://tinyurl.com/rv48628                                                                                                          
    https://communities.sas.com/t5/Statistical-Procedures/Meta-analysis-of-proportions-using-SAS/m-p/609444/highlight/true#M29510        
                                                                                                                                         
    *_                   _                                                                                                               
    (_)_ __  _ __  _   _| |_                                                                                                             
    | | '_ \| '_ \| | | | __|                                                                                                            
    | | | | | |_) | |_| | |_                                                                                                             
    |_|_| |_| .__/ \__,_|\__|                                                                                                            
            |_|                                                                                                                          
    ;                                                                                                                                    
                                                                                                                                         
    options validvarname=upcase;                                                                                                         
    libname sd1 "d:/sd1";                                                                                                                
    data sd1.have;                                                                                                                       
      retain country study total deaths;                                                                                                 
      informat study $14. country $15.;                                                                                                  
      input Study total deaths country;                                                                                                  
    cards4;                                                                                                                              
    Akenroye 3921 47 US                                                                                                                  
    Batra 4545 51 Australia                                                                                                              
    Berry2013 2939 0 US                                                                                                                  
    Berry2017 1699 50 US                                                                                                                 
    Blackburn 1055 53 US                                                                                                                 
    Cecil 4996 44 Europe                                                                                                                 
    Dosa 1430 0 US                                                                                                                       
    Edelson 4315 46 US                                                                                                                   
    Feinstein 4074 48 US                                                                                                                 
    Phelan 727 47 US                                                                                                                     
    Hudgins 1740 46 US                                                                                                                   
    Kuo 2626 49 US                                                                                                                       
    Massin 1048 0 Europe                                                                                                                 
    Noori 2979 48 Australia                                                                                                              
    Marsh 1424 64 US                                                                                                                     
    Montalbano 4849 50 US                                                                                                                
    Neuman 1608 47 US                                                                                                                    
    Peltz 4659 47 US                                                                                                                     
    Seo 2778 42 Korea                                                                                                                    
    Spaite 800 0 US                                                                                                                      
    Wijlaars2015 4573 0 Europe                                                                                                           
    Wijlaars2018 4941 57 Europe                                                                                                          
    Zook 4281 47 US US                                                                                                                   
    ;;;;                                                                                                                                 
    run;quit;                                                                                                                            
                                                                                                                                         
    SD1.HAVE total obs=23                                                                                                                
                                                                                                                                         
    Obs    COUNTRY      STUDY           TOTAL    DEATHS                                                                                  
                                                                                                                                         
      1    US           Akenroye         3921      47                                                                                    
      2    Australia    Batra            4545      51                                                                                    
      3    US           Berry2013        2939       0                                                                                    
      4    US           Berry2017        1699      50                                                                                    
      5    US           Blackburn        1055      53                                                                                    
      6    Europe       Cecil            4996      44                                                                                    
      7    US           Dosa             1430       0                                                                                    
      8    US           Edelson          4315      46                                                                                    
      9    US           Feinstein        4074      48                                                                                    
     10    US           Phelan            727      47                                                                                    
     11    US           Hudgins          1740      46                                                                                    
     12    US           Kuo              2626      49                                                                                    
     13    Europe       Massin           1048       0                                                                                    
     14    Australia    Noori            2979      48                                                                                    
     15    US           Marsh            1424      64                                                                                    
     16    US           Montalbano       4849      50                                                                                    
     17    US           Neuman           1608      47                                                                                    
     18    US           Peltz            4659      47                                                                                    
     19    Korea        Seo              2778      42                                                                                    
     20    US           Spaite            800       0                                                                                    
     21    Europe       Wijlaars2015     4573       0                                                                                    
     22    Europe       Wijlaars2018     4941      57                                                                                    
     23    US           Zook             4281      47                                                                                    
                                                                                                                                         
                                                                                                                                         
    *            _               _                                                                                                       
      ___  _   _| |_ _ __  _   _| |_                                                                                                     
     / _ \| | | | __| '_ \| | | | __|                                                                                                    
    | (_) | |_| | |_| |_) | |_| | |_                                                                                                     
     \___/ \__,_|\__| .__/ \__,_|\__|                                                                                                    
                    |_|                                                                                                                  
    ;                             Proportion       95%-CI                                                                                
                                                                                                                                         
    Overall probability of Death   0.013        [0.012, 0.014]                                                                           
                                                                                                                                         
    WORK.WANT total obs=40                                                                                                               
                                                                                                                                         
    Obs                                           LINES                                                                                  
                                                                                                                                         
      1    Study          Deaths Total         Proportion       95%-CI                                                                   
                                                                                                                                         
      2    Setting: US                                                                                                                   
      3    Akenroye              47   3921          0.012 [0.009, 0.016]                                                                 
      4    Berry2013              0   2939          0.000 [0.000, 0.001]                                                                 
      5    Berry2017             50   1699          0.029 [0.022, 0.039]                                                                 
      6    Blackburn             53   1055          0.050 [0.038, 0.065]                                                                 
      7    Dosa                   0   1430          0.000 [0.000, 0.003]                                                                 
      8    Edelson               46   4315          0.011 [0.008, 0.014]                                                                 
      9    Feinstein             48   4074          0.012 [0.009, 0.016]                                                                 
     10    Phelan                47    727          0.065 [0.048, 0.085]                                                                 
     11    Hudgins               46   1740          0.026 [0.019, 0.035]                                                                 
     12    Kuo                   49   2626          0.019 [0.014, 0.025]                                                                 
     13    Marsh                 64   1424          0.045 [0.035, 0.057]                                                                 
     14    Montalbano            50   4849          0.010 [0.008, 0.014]                                                                 
     15    Neuman                47   1608          0.029 [0.022, 0.039]                                                                 
     16    Peltz                 47   4659          0.010 [0.007, 0.013]                                                                 
     17    Spaite                 0   800           0.000 [0.000, 0.005]                                                                 
     18    Zook                  47   4281          0.011 [0.008, 0.015]                                                                 
     19    Subtotal                  42147          0.015 [0.014, 0.016]                                                                 
     20    Heterogeneity: I 2 = 99%, p < 0.01                                                                                            
                                                                                                                                         
     21    Setting: Australia                                                                                                            
     22    Batra                 51   4545          0.011 [0.008, 0.015]                                                                 
     23    Noori                 48   2979          0.016 [0.012, 0.021]                                                                 
     24    Subtotal                   7524          0.013 [0.011, 0.016]                                                                 
     25    Heterogeneity: I 2 = 39%, p = 0.07                                                                                            
                                                                                                                                         
     26    Setting: Europe                                                                                                               
     27    Cecil                 44   4996          0.009 [0.006, 0.012]                                                                 
     28    Massin                 0   1048          0.000 [0.000, 0.004]                                                                 
     29    Wijlaars2015           0   4573          0.000 [0.000, 0.001]                                                                 
     30    Wijlaars2018          57   4941          0.012 [0.009, 0.015]                                                                 
     31    Subtotal                  15558          0.006 [0.005, 0.008]                                                                 
                                                                                                                                         
     32    Heterogeneity: I 2 = 99%, p = 0.61                                                                                            
     33    Setting: Korea                                                                                                                
     34    Seo                   42   2778          0.015 [0.011, 0.020]                                                                 
     35    Subtotal                   2778          0.015 [0.011, 0.020]                                                                 
     36    Heterogeneity: not applicable                                                                                                 
                                                                                                                                         
     37    Total                    68007           0.013 [0.012, 0.014]                                                                 
     38    Heterogeneity: I 2 = 99%, p < 0.01                                                                                            
     39    Residual heterogeneity: I 2 = 93%,     0.02                                                                                   
                                                                                                                                         
    *                                                                                                                                    
     _ __  _ __ ___   ___ ___  ___ ___                                                                                                   
    | '_ \| '__/ _ \ / __/ _ \/ __/ __|                                                                                                  
    | |_) | | | (_) | (_|  __/\__ \__ \                                                                                                  
    | .__/|_|  \___/ \___\___||___/___/                                                                                                  
    |_|                                                                                                                                  
    ;                                                                                                                                    
                                                                                                                                         
    %utl_submit_r64('                                                                                                                    
    library(meta);                                                                                                                       
    library(haven);                                                                                                                      
    library(metafor);                                                                                                                    
    library(SASxport);                                                                                                                   
    library(haven);                                                                                                                      
    have<-read_sas("d:/sd1/have.sas7bdat");                                                                                              
    studies <- have$STUDY;                                                                                                               
    obs     <- have$DEATHS;                                                                                                              
    denom   <- have$SAMPLE;                                                                                                              
    setting <- have$COUNTRY;                                                                                                             
    m1 <- metaprop(obs, denom, studies, comb.random=F, byvar=setting,                                                                    
                   bylab="Setting", byseparator=": ");                                                                                   
    m2 <- metaprop(obs, denom, studies, comb.random=F, byvar=setting,                                                                    
                   bylab="Setting", byseparator=": ", method="GLMM");                                                                    
    m2$w.fixed <- m1$w.fixed;                                                                                                            
    pdf("d:/pdf/forest.pdf",width = 8, height =10);                                                                                      
    forest(m2, print.tau2 = FALSE, col.by="black", text.fixed = "Total",                                                                 
           text.fixed.w = "Subtotal", rightcols = c("effect","ci"), digits=3L,                                                           
           leftlabs=c("Study","Deaths","Total"));                                                                                        
    str(m2);                                                                                                                             
    pdf();                                                                                                                               
    ');                                                                                                                                  
                                                                                                                                         
                                                                                                                                         
    * scape the pdf to create want SAS dataset;                                                                                          
    %utl_submit_r64('                                                                                                                    
    library("tm");                                                                                                                       
    library(SASxport);                                                                                                                   
    file <- "d:/pdf/forest.pdf";                                                                                                         
    Rpdf <- readPDF(control = list(text = "-layout"));                                                                                   
    corpus <- VCorpus(URISource(file),                                                                                                   
          readerControl = list(reader = Rpdf));                                                                                          
    want <- as.data.frame(content(content(corpus)[[1]]));                                                                                
    colnames(want)<-"lines";                                                                                                             
    lines <- as.data.frame(strsplit(as.character(want$lines), split="\\r\\n"));                                                          
    colnames(lines)<-"lines";                                                                                                            
    str(lines);                                                                                                                          
    lines[] <- lapply(lines, function(x) if(is.factor(x)) as.character(x) else x);                                                       
    write.xport(lines,file="d:/xpt/lines.xpt");                                                                                          
    ');                                                                                                                                  
                                                                                                                                         
    * convert from VR transport to SAS dataset;                                                                                          
    libname xpt xport "d:/xpt/lines.xpt";                                                                                                
    data want;                                                                                                                           
      set xpt.lines;                                                                                                                     
    run;quit;                                                                                                                            
    libname xpt clear;                                                                                                                   
                                                                                                                                         
                                                                                                                                         
                                                                                                                                         
