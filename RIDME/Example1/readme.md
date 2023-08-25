# Example 1
## Simple analysis of a RIDME trace using standard DeerLab tools

This example was shown and discussed during the RIDME tutorial @ EFEPR 9th Summer School, Geneva, 2023. The attached data is an actually measured experimental result.

### Introduction
Basic analysis of RIDME trace almost does not deviate from that of 4p-DEER trace. The experimental signal $V(t)$ is represented as a product of intra-molecular dipolar form-factor $F(t)$ and intermolecular background decay $B(t)$
$$V(t) = F(t)\cdot B(t).$$

Although the theory of the form-factor is not the subject of the present example, it is worth to mention itw two important features that distinguish RIDME from DEER. Less orientation selection [Ritsch PCCP] but more complicated powder pattern that carries information on g-anisotropy [Millikisyants, Abdullin].

Another important difference is in the structure of the background factor. Besides the contribution from distant electrons (so-called dipolar background [Keller PCCP]) there is a substantial influence from close protons [Kuzin PCCP]. For that reason, one actively uses stretched exponential function ($\exp(-(kt)^{d/3})$ a.k.a. $\exp(-(t/T_{m})^{\xi}$ etc; `dl.bg_strexp` in DeerLab) to fit the background. In fully protonated samples, as exploited in this demonstration, one may expect the power to be close to 2 ($\xi\approx 2$ or $d\approx 6$).

### Code structure
...

### Typical output
![example output](./output1.png)

```r
Model parameters: 
=========== ======= ========================= ====== ====================================== 
 Parameter   Value   95%-Confidence interval   Unit   Description                           
=========== ======= ========================= ====== ====================================== 
 mod         0.294   (0.271,0.318)                    Modulation depth                      
 reftime     0.413   (0.413,0.414)              μs    Refocusing time                       
 decay       0.838   (0.801,0.875)             μs⁻¹   Decay rate                            
 stretch     2.049   (1.869,2.228)                    Stretch factor                        
 P           ...     (...,...)                 nm⁻¹   Non-parametric distance distribution  
 P_scale     0.995   (0.987,1.003)             None   Normalization factor of P             
=========== ======= ========================= ====== ====================================== 
```
Exchange interaction [Ritsch, Keller, PCCP].

### Outlook

### License

Designed and prepared by Sergei Kuzin, ETH Zurich. Free to use, modify and share.