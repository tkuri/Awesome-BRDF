# Awesome-BRDF
List of awesome papers on BRDF

## Table of contents

- [BRDF Representation](#brdf-representation)

## BRDF Representation
<img src="img/brdf.jpg" width=60%>

|Year|Pub|Name|Paper|Reciprocity|Energy Cons.|
|:---:|:---:|:---:|:---:|:---:|:---:|
|1720|Eberhard Klett|Lambert|[Photometria sive de mensura et gradibus luminis, colorum et umbrae](https://archive.org/details/lambertsphotome00lambgoog/page/n6/mode/2up)|||
|1975|CACM|Phong|[Illumination for computer generated pictures](https://dl.acm.org/doi/10.1145/360825.360839)|||
|1977|SIGGRAPH|Blinn-Phong|[Models of light reflection for computer synthesized pictures](https://dl.acm.org/doi/10.1145/965141.563893)|||
|1982|TOG|Cook-Torrance|[A Reflectance Model for Computer Graphics](https://dl.acm.org/doi/10.1145/357290.357293)||&#10003;||
|1991|SIGGRAPH|He|[A comprehensive physical model for light reflection](https://dl.acm.org/doi/10.1145/127719.122738)|&#10003;|&#10003;|
|1992|SIGGRAPH|Ward|[Measuring and modeling anisotropic reflection](https://dl.acm.org/doi/10.1145/142920.134078)|&#10003;||
|1994|SIGGRAPH|Oren-Nayar|[Generalization of Lambert's reflectance model](https://dl.acm.org/doi/10.1145/192161.192213)|&#10003;|&#10003;|
|1997|SIGGRAPH|Lafortune|[Non-Linear Approximation of Reflectance Functions](http://www.lafortune.eu/publications/Siggraph.html)|&#10003;|&#10003;|
|1999|CGF|Neumann|[Compact Metallic Reflectance Models](http://citeseer.ist.psu.edu/viewdoc/download;jsessionid=3D3407B845B0B7F0314B4D2694501DEE?doi=10.1.1.41.3489&rep=rep1&type=pdf)|&#10003;|&#10003;|
|2000|JGT|Ashikhmin-Shirley|[An anisotropic phong BRDF model](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.18.4558&rep=rep1&type=pdf)|||
|2001|CGF|Ershov|[Rendering pearlescent appearance based on paint-composition modelling](https://domino.mpi-inf.mpg.de/intranet/ag4/ag4publ.nsf/93832a04987390a3c12567530068622d/9bfb2b24db8e17bbc1256a7d004f1487/$FILE/EG01Paint.pdf)||&#10003;|
|2006|TOG|Edwards|[The halfway vector disk for brdf modeling](https://graphics.stanford.edu/~boulos/papers/brdftog.pdf)||&#10003;|
|2007|-|Ashikhmin-Premoze|[Distribution-based brdfs](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.621.5638&rep=rep1&type=pdf)|&#10003;|&#10003;|
|2007|EGSR|Walter(GGX)|[Microfacet Models for Refraction through Rough Surfaces](https://www.cs.cornell.edu/~srm/publications/EGSR07-btdf.html)|&#10003;|&#10003;|
|2008|GRAPHITE|Weidlich and Wilkie|[Arbitrarily Layered Micro-Facet Surfaces](https://www.cg.tuwien.ac.at/research/publications/2007/weidlich_2007_almfs/weidlich_2007_almfs-paper.pdf)|&#10003;|&#10003;|
|2010|SIGGRAPH|Kurt|[An anisotropic brdf model for fitting and monte carlo rendering](http://akademik.ube.ege.edu.tr/~kurt/Publications/SIGGRAPH_Computer_Graphics_2010_Kurt.pdf)|&#10003;|&#10003;|
|2012|CGF|Bagher|[Accurate fitting of measured reflectances using a Shifted Gamma micro-facet distribution](https://hal.inria.fr/hal-00702304/document)|&#10003;||
|2012|TOG|L&omacr;w|[Brdf models for accurate and efficient rendering of glossy surfaces](https://dl.acm.org/doi/10.1145/2077341.2077350)|&#10003;||
|2014|TOG|Brady|[genBRDF: discovering new analytic BRDFs with genetic programming](https://dl.acm.org/doi/10.1145/2601097.2601193)|&#10003;||
|2014|TOG|Jakob|[Discrete stochastic microfacet models](https://dl.acm.org/doi/10.1145/2601097.2601186)|||

### Fresnel Term
<img src=
"https://render.githubusercontent.com/render/math?math=%5Clarge+%5Cdisplaystyle+%5Cbegin%7Balign%2A%7D%0AF%3DF_0%2B%281-F_0%29%281-%5Ccos%7B%5Ctheta_i%7D%29%0A%5Cend%7Balign%2A%7D" 
alt="\begin{align*}
F=F_0+(1-F_0)(1-\cos{\theta_i})
\end{align*}">
<table>
  <thead>
  <tr>
    <th>Name</th>
    <th>Year</th>
    <th>Pub</th>
    <th>Paper</th>
    <th>Reciprocity</th>
    <th>Energy Cons.</th>
  </tr>
  </thead>
  <tbody>
  <tr>
    <td rowspan="2">Lambert</td>
    <td>1720</td>
    <td>Eberhard Klett</td>
    <td><a href= "https://archive.org/details/lambertsphotome00lambgoog/page/n6/mode/2up">Photometria sive de mensura et gradibus luminis, colorum et umbrae</a></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td colspan='5'><img src=
"https://render.githubusercontent.com/render/math?math=%5Clarge+%5Cdisplaystyle+%5Cbegin%7Balign%2A%7D%0A%5Cfrac%7B1%7D%7B%5Cpi%7D%5Crho_d%0A%5Cend%7Balign%2A%7D%0A" 
alt="\begin{align*}
\frac{1}{\pi}\rho_d
\end{align*}
"></td>
  </tr>
  <tr>
    <td rowspan="2">Phong</td>
    <td>1975</td>
    <td>CACM</td>
    <td>
    <a href="https://dl.acm.org/doi/10.1145/360825.360839">Illumination for computer generated pictures</a>
    </td>
    <td></td>
    <td></td>
  </tr>
  <tr>
  <td colspan='5'><img src="https://render.githubusercontent.com/render/math?math=%5Clarge+%5Cdisplaystyle+%5Cbegin%7Balign%2A%7D%0Ai_d+%2B+%5Crho_s%28%5Comega_o+%5Ccdot+%5Comega_r%29%5Em%0A%5Cend%7Balign%2A%7D%0A" alt="\begin{align*}i_d + \rho_s(\omega_o \cdot \omega_r)^m\end{align*}"></td>
  </tr>
  <tr>
    <td rowspan="2">Blinn-Phong</td>
    <td>1977</td>
    <td>SIGGRAPH</td>
    <td>
    <a href="https://dl.acm.org/doi/10.1145/965141.563893">Models of light reflection for computer synthesized pictures</a>
    </td>
    <td></td>
    <td></td>
  </tr>
  <tr>
  <td colspan='5'><img src="https://render.githubusercontent.com/render/math?math=%5Clarge+%5Cdisplaystyle+%5Cbegin%7Balign%2A%7D%0Ai_d%2B%5Crho_s%28%5Cmathbf%7Bn%7D+%5Ccdot+%5Cmathbf%7Bh%7D%29%5Em%0A%5Cend%7Balign%2A%7D" 
alt="\begin{align*}i_d+\rho_s(\mathbf{n} \cdot \mathbf{h})^m\end{align*}"></td>
  </tr>
  <tr>
    <td rowspan="2">Cook-Torrance</td>
    <td>1977</td>
    <td>SIGGRAPH</td>
    <td>
    <a href="https://dl.acm.org/doi/10.1145/357290.357293">A Reflectance Model for Computer Graphics</a>
    </td>
    <td align="center">&#10003;</td>
    <td></td>
  </tr>
  <tr>
  <td colspan='5'><img src="https://render.githubusercontent.com/render/math?math=%5Clarge+%5Cdisplaystyle+%5Cbegin%7Balign%2A%7D%0Ai_d%2B%5Crho_s%5Cfrac%7BDGF%7D%7B%5Cpi%28%5Cmathbf%7Bn%7D+%5Ccdot+%5Comega_i%29%28%5Cmathbf%7Bn%7D+%5Ccdot+%5Comega_o%29%7D%0A%5Cend%7Balign%2A%7D" alt="\begin{align*}i_d+\rho_s\frac{DGF}{\pi(\mathbf{n} \cdot \omega_i)(\mathbf{n} \cdot \omega_o)}\end{align*}">
<img src=
"https://render.githubusercontent.com/render/math?math=%5Clarge+%5Cdisplaystyle+%5Cbegin%7Balign%2A%7D%0AD%3D%5Cfrac%7B1%7D%7B4m%5E2%28%5Cmathbf%7Bn%7D+%5Ccdot+%5Cmathbf%7Bh%7D%29%5E4%7D%5Cexp%7B%5CBigg%28-%5Cfrac%7B1-%28%5Cmathbf%7Bn%7D+%5Ccdot+%5Cmathbf%7Bh%7D%29%5E2%7D%7Bm%5E2%28%5Cmathbf%7Bn%7D+%5Ccdot+%5Cmathbf%7Bh%7D%29%5E2%7D%5CBigg%29%7D%0A%5Cend%7Balign%2A%7D" 
alt="\begin{align*}
D=\frac{1}{4m^2(\mathbf{n} \cdot \mathbf{h})^4}\exp{\Bigg(-\frac{1-(\mathbf{n} \cdot \mathbf{h})^2}{m^2(\mathbf{n} \cdot \mathbf{h})^2}\Bigg)}
\end{align*}">
<img src=
"https://render.githubusercontent.com/render/math?math=%5Clarge+%5Cdisplaystyle+%5Cbegin%7Balign%2A%7D%0AG%3D%5Cmin%7B%5CBigg%281%2C+%5Cfrac%7B2%28%5Cmathbf%7Bn%7D+%5Ccdot+%5Cmathbf%7Bh%7D%29%28%5Cmathbf%7Bn%7D+%5Ccdot+%5Cmathbf%7B%5Comega_o%7D%29%7D%7B%5Cmathbf%7Bh%7D+%5Ccdot+%5Comega_o%7D%2C+%5Cfrac%7B2%28%5Cmathbf%7Bn%7D+%5Ccdot+%5Cmathbf%7Bh%7D%29%28%5Cmathbf%7Bn%7D+%5Ccdot+%5Cmathbf%7B%5Comega_i%7D%29%7D%7B%5Cmathbf%7Bh%7D+%5Ccdot+%5Comega_o%7D%5CBigg%29%7D%0A%5Cend%7Balign%2A%7D" 
alt="\begin{align*}
G=\min{\Bigg(1, \frac{2(\mathbf{n} \cdot \mathbf{h})(\mathbf{n} \cdot \mathbf{\omega_o})}{\mathbf{h} \cdot \omega_o}, \frac{2(\mathbf{n} \cdot \mathbf{h})(\mathbf{n} \cdot \mathbf{\omega_i})}{\mathbf{h} \cdot \omega_o}\Bigg)}
\end{align*}">
    </td>
  </tr>
  <tr>
    <td rowspan="2">He</td>
    <td>1991</td>
    <td>SIGGRAPH</td>
    <td>
    <a href="https://dl.acm.org/doi/10.1145/127719.122738">A comprehensive physical model for light reflection</a>
    </td>
    <td align="center">&#10003;</td>
    <td align="center">&#10003;</td>
  </tr>
  <tr>
  <td colspan='5'>
  </td>
  </tr>        
  <tr>
    <td rowspan="2">Ward</td>
    <td>1992</td>
    <td>SIGGRAPH</td>
    <td>
    <a href="https://dl.acm.org/doi/10.1145/142920.134078">Measuring and modeling anisotropic reflection</a>
    </td>
    <td align="center">&#10003;</td>
    <td align="center"></td>
  </tr>
  <tr>
  <td colspan='5'>
    <img src=
"https://render.githubusercontent.com/render/math?math=%5Clarge+%5Cdisplaystyle+%5Cbegin%7Balign%2A%7D%0AD_%7Biso%7D%3D%5Cfrac%7B1%7D%7B4+%5Cpi+m%5E2+%5Csqrt%7B%28%5Cmathbf%7Bn%7D+%5Ccdot+%5Comega_i%29%28%5Cmathbf%7Bn%7D+%5Ccdot+%5Comega_o%29%7D%7D%5Cexp%7B%5CBig%28-%5Ctan%5E2+%5CBig%28%5Cfrac%7B%5Ctheta_h%7D%7Bm%5E2%7D%5CBig%29%5CBig%29%7D%0A%5Cend%7Balign%2A%7D" 
alt="\begin{align*}
D_{iso}=\frac{1}{4 \pi m^2 \sqrt{(\mathbf{n} \cdot \omega_i)(\mathbf{n} \cdot \omega_o)}}\exp{\Big(-\tan^2 \Big(\frac{\theta_h}{m^2}\Big)\Big)}
\end{align*}">
    <img src=
"https://render.githubusercontent.com/render/math?math=%5Clarge+%5Cdisplaystyle+%5Cbegin%7Balign%2A%7D%0AD_%7Baniso%7D%3D%5Cfrac%7B1%7D%7B4+%5Cpi+m_x+m_y+%5Csqrt%7B%28%5Cmathbf%7Bn%7D+%5Ccdot+%5Comega_i%29%28%5Cmathbf%7Bn%7D+%5Ccdot+%5Comega_o%29%7D%7D%5Cexp%7B%5CBigg%28-%5Ctan%5E2%28%5Ctheta_h%29+%5CBig%28%5Cfrac%7B%28%5Cmathbf%7Bh%7D+%5Ccdot+%5Comega_i%29%7D%7Bm_x%5E2%7D%2B%5Cfrac%7B%28%5Cmathbf%7Bh%7D+%5Ccdot+%5Comega_i%29%7D%7Bm_y%5E2%7D%5CBig%29%5CBigg%29%7D%0A%5Cend%7Balign%2A%7D" 
alt="\begin{align*}
D_{aniso}=\frac{1}{4 \pi m_x m_y \sqrt{(\mathbf{n} \cdot \omega_i)(\mathbf{n} \cdot \omega_o)}}\exp{\Bigg(-\tan^2(\theta_h) \Big(\frac{(\mathbf{h} \cdot \omega_i)}{m_x^2}+\frac{(\mathbf{h} \cdot \omega_i)}{m_y^2}\Big)\Bigg)}
\end{align*}">
  </td>
  </tr>        
  <tr>
    <td rowspan="2">Oren-Nayar</td>
    <td>1994</td>
    <td>SIGGRAPH</td>
    <td>
    <a href="https://dl.acm.org/doi/10.1145/192161.192213">Generalization of Lambert's reflectance model</a>
    </td>
    <td align="center">&#10003;</td>
    <td align="center">&#10003;</td>
  </tr>
  <tr>
  <td colspan='5'>
    <img src=
"https://render.githubusercontent.com/render/math?math=%5Clarge+%5Cdisplaystyle+%5Cbegin%7Balign%2A%7D%0Ai_d%3D%5Crho_d+%5Cfrac%7B1%7D%7B%5Cpi%7D%5CBig%281-%5Cfrac%7B0.5%7D%7Bm%2B0.33%7D%2B%5Cfrac%7B0.44m%7D%7Bm%2B0.99%7D%5Ccos%7B%28%5Cphi_i-%5Cphi_o%29%7D%5Csin%7B%5Cbig%28%5Cmax%7B%28%5Ctheta_i%2C+%5Ctheta_o%29%7D%5Cbig%29%7D%5Ctan%7B%5Cbig%28%5Cmin%7B%28%5Ctheta_i%2C+%5Ctheta_o%29%7D%5Cbig%29%7D%5CBig%29%0A%5Cend%7Balign%2A%7D" 
alt="\begin{align*}
i_d=\rho_d \frac{1}{\pi}\Big(1-\frac{0.5}{m+0.33}+\frac{0.44m}{m+0.99}\cos{(\phi_i-\phi_o)}\sin{\big(\max{(\theta_i, \theta_o)}\big)}\tan{\big(\min{(\theta_i, \theta_o)}\big)}\Big)
\end{align*}">
  </td>
  </tr>
  <tr>
    <td rowspan="2">Lafortune</td>
    <td>1997</td>
    <td>SIGGRAPH</td>
    <td>
    <a href="http://www.lafortune.eu/publications/Siggraph.html">Non-Linear Approximation of Reflectance Functions</a>
    </td>
    <td align="center">&#10003;</td>
    <td align="center">&#10003;</td>
  </tr>
  <tr>
  <td colspan='5'>
  </td>
  </tr>
  <tr>
    <td rowspan="2">Neumann</td>
    <td>1999</td>
    <td>CGF</td>
    <td>
    <a href="http://citeseer.ist.psu.edu/viewdoc/download;jsessionid=3D3407B845B0B7F0314B4D2694501DEE?doi=10.1.1.41.3489&rep=rep1&type=pdf">Compact Metallic Reflectance Models</a>
    </td>
    <td align="center">&#10003;</td>
    <td align="center">&#10003;</td>
  </tr>
  <tr>
  <td colspan='5'>
  </td>
  </tr>
  <tr>
    <td rowspan="2">Ashikhmin-Shirley</td>
    <td>2000</td>
    <td>JGT</td>
    <td>
    <a href="http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.18.4558&rep=rep1&type=pdf">An anisotropic phong BRDF model</a>
    </td>
    <td align="center"></td>
    <td align="center"></td>
  </tr>
  <tr>
  <td colspan='5'>
  </td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>


</tbody>
</table>
