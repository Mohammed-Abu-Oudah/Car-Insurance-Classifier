# Car-Insurance-Classifier

The data seemed really interesting.
We extracted the first top 2 important features.

which are driving experience and vehical ownership.
here's is the plot showing the importance of the top10 most important features.<br/>
<img width="830" height="547" alt="download" src="https://github.com/user-attachments/assets/cc19b5e5-b877-4874-8990-003bd882e74c" />

adding to that here is the plot of target against the driving experience feature.<br/>
<img width="590" height="390" alt="download" src="https://github.com/user-attachments/assets/4ac29dc0-34c9-418d-98d0-2a7c8318e3a7" />

and here's the plot of target against the vehical ownership.<br/>
<img width="536" height="393" alt="download" src="https://github.com/user-attachments/assets/300e66f1-f914-4975-843b-5cc2474f8a39" />

Now we moved to the unsupervised machine learning to test how it would work with this data.<br/>
We observed the Inirtia values and the Silhouette scores for different numbers of clusters as demostrated in the figures below <br/>
<img width="597" height="432" alt="download" src="https://github.com/user-attachments/assets/48a000ae-2d5d-4fc3-80fa-565eb67fb844" />
<img width="576" height="432" alt="download" src="https://github.com/user-attachments/assets/975cf52b-c528-4304-919c-96564de723b3" />

after that, we found that the Silhouette scores were low in general so we decided to check the source of the problem and it was noticed in the 3D graphs that when creating a scatter based on the 3 PCs we had, the level of separation between the clusters and the cohesion of the one cluster were very high.<br/>

For that reason we decided to move back to the classification methods but with a small tweak which was adding the forward feature selection algorithm which resulted in selecting the best features, causing the model to eleminate the overfit and provide us with a significantly imporved performance as demostrated in the following figures.

<img width="917" height="687" alt="image" src="https://github.com/user-attachments/assets/2c9cb83e-ac1d-417e-b92c-7e0f35639095" />
<img width="947" height="657" alt="image" src="https://github.com/user-attachments/assets/a176a961-3482-4d0f-9a8e-14f7943e9aec" />



