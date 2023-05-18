---
layout: page
title: Hands-on Workshop on diffusion MRI
image: assets/images/IberianISMRM2023_workshop.png
summary: "3rd ISMRM Iberian Chapter annual meeting | July 3-5, 2023 | Valladolid, Spain"
---

<img src="{{ site.baseurl }}/assets/images/IberianISMRM2023_workshop.png" width="100%"/>


# **Topics:**
   - Diffusion MRI<br>
   - Advanced metrics<br>
   - Microstructure<br>
   - Software<br>
   - Biomarkers for brain studies<br>


# **Organizers:**
Laboratorio de Procesado de Imagen, LPI, Universidad de Valladolid, Spain<br>
<a href="http://www.lpi.tel.uva.es">http://www.lpi.tel.uva.es</a>

   - Santiago Aja-Fernández<br>
   - Antonio Tristán-Vega<br>   
   - Tomasz Pieciak<br>   



# **Registration**

<p>The participation in the workshop is included with the ISMRM Iberian chapter registration.</p>

### **Register for the hands-on workshops in diffusion MRI:** <a target="_blank" href="https://docs.google.com/forms/d/e/1FAIpQLSeAIgWvQxm73sbIo7zpmHMsGFjQpGebAJ0y_hFu-zx5OE26JQ/viewform">Click HERE</a>

### **Register for the Workshop:** <a target="_blank" href="https://docs.google.com/forms/d/e/1FAIpQLSeAIgWvQxm73sbIo7zpmHMsGFjQpGebAJ0y_hFu-zx5OE26JQ/viewform">Click HERE</a>


<p>&nbsp;</p>


# **Some background about the methods**

<p>Diffusion magnetic resonance imaging (dMRI) has gained much interest from the neuroimaging community over the last two decades, due to its ability to analyze in vivo structures within the white matter of the brain. These techniques are used by many prestigious international centers and have been the basis of major international projects in the last decades with millions of Euros of funding, such as the Human Brain Project (EU) or the NIH Human Connectome Project (USA). The current trend in dMRI analysis is the calculation of increasingly advanced metrics focused on subtle aspects of the diffusion and brain microstructure.<br><br></p>

<p>However, for the calculation of these advanced measures, the acquisition requirements may get higher and higher:<p>
   - Increasingly powerful MRI scanners, such as the Siemens 3T MAGNETOM Prisma (with a gradient power of 80mT/m), Siemens 3T Connectome (with a gradient power of 300mT/m) or commercial scanners up to 7T.<br>
   - Denser q-space sampling: higher number of shells (b-values) and higher number of samples per shell.<br><br>

<p>In the first case, there is a clear economic limitation: not all centers can afford such expensive dedicated equipment. For the second requirement, an increase in the number of samples at each acquisition leads to longer acquisition times. Thus, these techniques are not totally compatible with clinical and research acquisitions that can be performed in standard medical or research centers. In the standard case:</p>
   - Acquisitions must be performed within a preset time, for the patient's convenience and to take advantage of the scanners. Typically, studies are performed in addition to clinical acquisitions, so a patient cannot spend 2 hours inside the machine. For studies with a larger number of patients, this would simply imply times that cannot be afforded by the public health system.
   - The scanners available for research in most centers are those that are also used clinically. Many national centers already have 3T scanners (as opposed to the large number of 1.5T scanners still in use). However, there are no national centers with advanced scanners specialized for diffusion.

<p>These limitations could make it impossible for most national research and clinical centers to carry out state-of-the-art brain research using advanced diffusion metrics.<br></p>

<p>To alleviate this problem, the LPI (Valadolid) has been working for years on advanced measures that provide similar clinical information to existing ones but using commercial scanners and a limited number of samples. Several techniques have been proposed, based on different models. Methods are based on the reduction of the number of degrees of freedom of the estimation problem by introducing prior assumptions and thus reducing the minimum number of data needed for estimation. The main methods are:<br></p>

<p>1. Apparent Measures Using Reduced Acquisitions (AMURA). The method allows the direct estimation of diffusion measures such as RTOP, RTAP and PA, avoiding the calculation of the EAP while reducing the number of necessary samples and the computational cost. It assumes a behavior of the diffusion process that is roughly independent from the b-value. This assumption, common in high angular resolution diffusion imaging (HARDI) acquisitions, allows the calculation of these metrics from single-shell acquisitions, tipical in clinical routine. Since the assumed model only holds within a limited range around the b-value considered, the derived measures must be considered as apparent values at a given b-value, dependent on the selected shell. However, despite this dependence with the b-value, the apparent metrics calculated with AMURA have shown a good correlation with the same metrics calculated using standard multishell approaches.<br>

2. Micro-Structure-adaptive convolution kernels and dual Fourier domains Integral Transforms (MiSFIT). This technique calculates the EAP and then the metrics can be derived. As opposed to the related approaches in the state of the art, MiSFIT is not based on fitting the EAP in some functions basis, which makes it time efficient at the same time it relaxes the low-frequency constraints imposed by the maximum b-value acquired. Instead, it is based on convolution kernels and dual Fourier domains Integral Transforms. Due to the low-rank signal representation, with at most 3 parameters to estimate, it could provide a full representation of the EAP and all the scalar moments with just 2 shells (for the simplified representation) or 3 shells if free water is also estimated. At the same time, the decoupled optimization in a low rank non-linear problem for the radial behavior and a model-free, linear problem for the orientation makes MiSFIT extremely time-efficient, beating the computation times of other methods by two orders of magnitude.<br>

3. Hybrid Diffusion Imaging - Diffusion Spectrum Imaging - Quadratic Programming (HYDI-DSI-QP).  <br></p>


<p>&nbsp;</p>


# **About the Workshop**

<p>The organizing team has been working for years on advanced measures estimated from diffusion MRI that provide similar clinical information to existing ones but using commercial scanners and a limited number of samples. Several techniques have been proposed, based on different models. These are based on the reduction of the number of degrees of freedom of the estimation problem by introducing prior assumptions and thus reducing the minimum number of data needed for estimation. The metrics derived from the new methodologies can be used as biomarkers in different clinical studies.<br></p>

In this workshop:<br>
   - We will review the philosophy and models behind each method.<br>
   - We will explain the minimum acquisition requirements for the calculation of the metrics.<br>
   - Participants will be playing with the software to learn how to estimate the different metrics from real data.<br>

<p>&nbsp;</p>

# **Schedule**
   - 15:00 Presentation of the Workshop<br>
   - 15:15 General Description of the methods and models<br>
   - 16:00: Requirements for the calculation of the metrics<br>
   - 16:45 Coffee Break<br>
   - 17:00-18:30 Hands-on session<br>
   - 20:00 Tapas dinner<br>

<p>&nbsp;</p>

# **Resources**

   - Software and information about the methods: dMRILab, download it here: <a href="http://lpi.tel.uva.es/dmrilab">http://lpi.tel.uva.es/dmrilab</a><br>
   - References: A whole book with all the methods will be provided to the participants.<br><br>


IMPORTANT: The hands-on session will be carried out in MATLAB. If you do not have a computer with MATLAB, we can provide, but you should let us know beforehand.


