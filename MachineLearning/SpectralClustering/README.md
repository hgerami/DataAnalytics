<h2> Steps in Spectral Clustering: </h2>
<ul>
  <li> Step 1: build an adjacency matrix > using nearest neighbors </li>
  <li> Step 2: represent graph as adjacency matrix A </li>
  <li> Step 3: form a special matrix L = D - A, the graph Laplacian </li>
  <li> Step 4: compute k eigenvectors, corresponding to the k smallest eigenvalues </li>
  <li> Step 5: run kmeans algorithm on the k eigenvecotrs by treating each row as a new data point <li> </ul>
  
  <p><a href="SpectralClustering.ipynb"> Examples on Spectral Clustering </a></p>
  <p><b>Reference: ISyE 6740 Course Material, Yao Xie</b></P>
  
  
