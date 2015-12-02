
                                                                                                                                                                                                                            
                       N                                                                                                                                                                                                    
                        Z                                  ZZO                                                                    ZZO                                                                                       
             NOZZZZZZZZZ 7O                                ZZO                                                                    ZZO                                                                                       
       OZZZZZZZZZZZZZZZZO $$                               ZZO                                                                    ZZO                                                                                       
        NDN     8ZZZZZZZZ 7$$N                     NNNN    ZZO                               NNN                 NNNN             ZZO               NNNN         NNNN                 NNNN            NNNN                  
       $$$$$$$$7O   ZOZZZD $$$$                ZZZZZZZZZZZZZZO   OZZN          ZZZ    ZZZZZZZZZZZZZZO       ZZZZZZZZZZZZZ8    ZZZZZZZZZZZ     8ZZZZZZZZZ   ZZZZZZZZZZZZZO        DZZZZZZZZZZ      ZZZZZZZZZZZZN             
      8$$$$$$$$$8      ZZO Z$$$$              ZZZO        DZZO    OZZ         NZZD   NZZO         8ZZZ                 ZZZO       ZZO         ZZOD                    8ZZZN     OZZZN            ZZZN       OZZO            
      $$$$$7O            Z  $$$$$8           ZZZ           ZZO    NZZO        ZZZ    NZZN          NZZO                 OZZN      ZZO         ZZO                       ZZZ    DZZ8             ZZO          DZZZ           
     O$$$$Z                 $$$$$$           ZZO           ZZO     ZZZ       NZZD    NZZN           ZZZ                  ZZD      ZZO         ZZO                       ZZZ    ZZZ             8ZZ            ZZZ           
     7$$O  Z                $$$$$D Z        8ZZ            ZZO      $ZZ      ZZO     NZZ            ZZZ                 NZZD      ZZO         ZZO                       OZZ    ZZZ             ZZZ            ZZZ           
    7$$  ZZN                $$$$N O         OZZ            ZZO       ZZO    NZZN     NZZ            ZZZ      8ZZZZZZZZZZZZZD      ZZO         ZZO            ZZZZZZZZZZZZZZ    ZZO             ZZZ           NZZZN          
   N$8 ZZZZ                N$$$ NZO         ZZZ            ZZO       OZZ    ZZZ      NZZ            ZZZ    8ZZZN         ZZD      ZZO         ZZO          ZZZ8N        ZZZ    ZZO             ZZZZZZZZZZZZZZZZZZ           
   ZD ZZZZZ                $7  ZOO          8ZZ            ZZO        ZZZ  8ZZ       NZZ            ZZZ    ZZZ           ZZD      ZZO         ZZO         8ZZN          ZZZ    ZZZ             ZZZDN                        
   D ZZZZZZ               N  8ZZZZ          NZZN           ZZO        NZ$8 ZZZ       NZZ            ZZZ   8ZZN           ZZD      ZZO         ZZO         ZZZ           ZZZ    ZZZ             OZZ                          
    DZZZZZZ D              8ZZZZZ            ZZZ           ZZO         8ZZZZZ        NZZ            ZZZ   8ZZD           ZZD      ZZO         ZZO         ZZZ           ZZZ    DZZD             ZZ8                         
      ZZZZZ  $$         8ZZZZZZZO            8ZZZ          ZZ8          ZZZZZ        NZZ            ZZZ   NZZZ           ZZD      ZZZ         ZZO         OZZD          ZZZ     ZOZD            DZZZ                        
       ZZZZ8 7$$Z   8ZZZZZZZZZZZ              DZZZZON NDOZZZZ8           ZZO         NZZ            ZZZ    8ZZZO8NNNN8ZZZZZN      ZZZZ8NN     ZZO          ZOZZONNNNNOZZZZZ      ZZZZZO8N8OZ     OZZZZODNNN8OZZZN           
        8ZZZ O$$$$$Z    OZZZZZZ                 DZZZZZZZZZZD            NZZD         NZZ            ZZZ      DZZZZZZZZZZO          NZZZZZD    ZZO            OZZZZZZZZZZ8          ZZZZZZZZZD      8ZZZZZZZZZZZZ8           
          ZZN $$$$$$$$$7Z                                               ZZZ                                                                                                                                                 
           OZ D$$$$$$$$$$$7$D                                          NZZD                                                                                                                                                 
            DZ 7$$$7$ZN                                                ZOZ                                                                                                                                                  
              8                                                                                                                                                                                                             


        * * * * * * * * * * 
      ______________________                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      
/////Created by Brian Wilson\\\\\
     ------------------------
     ||                    ||     
           
This zip file contains to items.
	1 - the dynatrace sitecore fastpack (sitecore-fastpack-1.0.dtp) which gets deployed to the dynatrace server
	2 - the Dynatrace.PatchRenderings.zip which gets deployed to your sitecore instance using the Sitecore Installation Wizard.
	
The Dynatrace.PatchRenderings.zip contains 3 files:
	1 - dynatrace.config
	2 - dynatrace.patchRenderings.dll
	3 - dynatrace.patchRenderings.pdb
	
	The purpose of this package is to expose the following information to dynatrace utilizing 2 custom methods
	1 - CaptureInDTMain captures the following information for each page and can be found in the Dynatrace Business Transaction named Sitecore Main Layout 
		as well as the Dynatrace dashboard SiteCore Rendering Performance:
		* URL
		* ID
		* Name
		* DisplayName
	2 - CaptureInDTSub captures the following information for each rendering on the main page and can be found in the Dynatrace Business Transaction 
		named Sitecore Sublayouts as well as the Dynatrace dashboard SiteCore Rendering Performance:
		* Placeholder
		* ID
		* DisplayName
		* DataSource
		
If you choose not to deploy this package to sitecore, the above mentioned business transactions will not work and some content will be missing from the
	Dynatrace dashboard SiteCore Rendering Performance
	
	