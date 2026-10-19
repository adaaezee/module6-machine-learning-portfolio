# Reflective Piece

[← Back to e-portfolio](README.md)

*This reflection is also submitted separately as a Word document. It uses Rolfe et al.'s (2001) reflective model.*

Joining the Machine Learning module as part of my master's course has been both engaging and, at times, complex. In this piece I reflect on my involvement in the module and my contributions to the Development Team Project and my individual project, using Rolfe et al.'s (2001) What? So what? Now what? model. The module played an integral part in my growth as a Master's student, particularly because I was able to act on feedback from previous modules, which asked me to show more specific technical evidence and stronger ownership of my work.

## What?

Units 1 to 6 centred on the Development Team Project, in which our team of four analysed New York City Airbnb listings using regression and clustering. The project was exciting and engaging. Taking on the role of joint Project Lead and Coordinator came fairly naturally: as a manager at a technology company, organisation and delegation are strengths of mine, and it was rewarding to be part of a team who trusted me with this role. I shared the team contract, coordinated meetings through Telegram and arranged our early planning calls. All three of my teammates were productive to work with. Tasks were divided in a shared document, with everyone highlighting their strengths and weaknesses in our first meetings, so that each member could contribute where they were strongest.

Through that process I took ownership of the entire clustering section, which I carried out in R. Having previously used WEKA in an earlier MSc module to analyse financial transaction data and evaluate classification models, I felt confident taking this on. Although k-means clustering is an unsupervised approach, my familiarity with data preprocessing, feature selection and model evaluation gave me a useful foundation.

Outside the team project, I engaged with the module mainly through seminar recordings, lecturecasts, the reading and unit activities such as the Jaccard distance exercise, rather than by posting in the collaborative discussions. In Unit 11, I returned to the same dataset individually, comparing polynomial regression with a neural network using cross-validation, SHAP explanations and a subgroup bias analysis.

## So what?

Owning the clustering taught me to balance statistical performance with practical interpretation. Although k = 2 achieved a higher silhouette score (0.392) than k = 3 (0.252), I chose three clusters because they gave a more useful segmentation of listings. This showed me that model selection should not depend on evaluation metrics alone, but on the purpose of the analysis. However, the tutor's feedback that our clustering was “relatively brief”, with “limited interpretation” of how Airbnb could use the segments, was fair, and initially disappointing. I had justified my choice of k, then stopped at describing the clusters rather than asking what a business should do with them. Looking back, my long-stay cluster, whose hosts held a median of 16 listings, pointed to professional operators - a regulatory question as much as a pricing one.

That feedback shaped my Unit 11 project. When cross-validation showed the neural network failing on one fold (R² = 0.035), I felt uneasy, because the network had the better test score and a single train/test split would have hidden the failure. I recommended polynomial regression instead, because reliability and auditability matter more than a marginal gain in a tool that affects hosts' income. This is consistent with Shwartz-Ziv and Armon's (2022) finding that deep learning does not reliably outperform simpler models on tabular data. The subgroup analysis, which showed the highest error for the smallest boroughs and room types, turned a technical metric into an ethical question about who a model serves least well. I realised that the biggest change was in my process, as I had moved from describing what a model found to questioning whether it could be trusted.

Virtual teamwork taught me just as much. Working across time zones, full-time jobs and night shifts required adaptability, and we agreed early on that members who could not join a call would receive written updates. Each member brought different perspectives, which encouraged me to stay open to alternative approaches, for example when we resolved a debate about validation splits by returning to the course textbook. I also noticed that roles on paper differed from roles in practice: the contract also named me UML and Design Lead, yet my most valuable contribution became the technical analysis, and Sarah took over the meeting notes from late August. Finally, not posting in the discussion forums meant I missed the peer critique I had found extremely valuable in a previous module, which I would approach differently next time.

## Now what?

I will carry three key lessons forward. First, I will integrate practical interpretation throughout the analytical process rather than treating it as an afterthought, ensuring that findings provide meaningful insights for stakeholders. Second, I will prioritise robust model validation and explainability, recognising that individual performance metrics may conceal underlying weaknesses. Third, I will consider algorithmic fairness across demographic subgroups as an essential requirement when evaluating AI systems.

These lessons will directly inform my final module, the Computing Project, where I intend to investigate employee trust in AI-enabled biometric access control systems. Given the recognised challenges surrounding interpretability, privacy and generalisation across diverse populations (Achimba et al., 2025), I aim to apply these principles when evaluating the transparency, fairness and trustworthiness of such systems.

Professionally, I aim to move into AI transformation roles within technology or other forward-thinking sectors. This module showed me that the value I can bring lies not only in building models, but in connecting their results to business decisions and leading teams through the questions those models raise. To support this, I intend to continue building my independent coding confidence and to contribute more actively to peer discussion.

Overall, the experience taught me that successful machine-learning projects require not only technical competence, but also critical evaluation, effective communication and an understanding of how analytical findings translate into real-world applications.

## References

Achimba, T., Okhuoya, O.J., Akinyede, R.O., Ibrahim, A., Alabi, P.A. and Ateata, G. (2025) ‘A robust biometric authentication framework for access control’, University of Ibadan Journal of Science and Logics in ICT Research, 13(1), pp. 239–246.

Rolfe, G., Freshwater, D. and Jasper, M. (2001) Critical reflection in nursing and the helping professions: a user’s guide. Basingstoke: Palgrave Macmillan.

Shwartz-Ziv, R. and Armon, A. (2022) ‘Tabular data: deep learning is not all you need’, Information Fusion, 81, pp. 84–90.
