<!DOCTYPE html>
<html lang="en">


<h1>Star, Quasar, and Galaxy Detection Using SVM and Random Forest</h1>

<h2>Overview</h2>
<p>This project analyzes astronomical observations from the Sloan Digital Sky Survey (SDSS) to classify objects in the universe into three categories: <strong>Star</strong>, <strong>Galaxy</strong>, and <strong>Quasar</strong>. The SDSS has created the most detailed three-dimensional maps of the Universe, providing deep multi-color images and spectra for over three million astronomical objects.</p>

<h2>Data Description</h2>
<p>The dataset consists of <strong>10,000 observations</strong> of space, each described by <strong>17 feature columns</strong> and <strong>1 class column</strong>. The class column identifies the object as either a Star, Galaxy, or Quasar.</p>

<h3>Features</h3>
<p>The dataset includes the following features:</p>
<ul>
    <li><code>objid</code>: A unique identifier for each object in the dataset.</li>
    <li><code>ra</code> (Right Ascension): The celestial coordinate specifying the object's position in the sky (in degrees).</li>
    <li><code>dec</code> (Declination): The celestial coordinate specifying the object's position in the sky (in degrees).</li>
    <li><code>u</code>: Magnitude of the object in the ultraviolet filter (360-400 nm).</li>
    <li><code>g</code>: Magnitude of the object in the green filter (400-550 nm).</li>
    <li><code>r</code>: Magnitude of the object in the red filter (550-700 nm).</li>
    <li><code>i</code>: Magnitude of the object in the infrared filter (700-900 nm).</li>
    <li><code>z</code>: Magnitude of the object in the far-red filter (900-1100 nm).</li>
    <li><code>run</code>: The run number of the observation.</li>
    <li><code>rerun</code>: The rerun number of the observation.</li>
    <li><code>camcol</code>: The camera column number used for the observation.</li>
    <li><code>field</code>: The field number of the observation.</li>
    <li><code>specobjid</code>: A unique identifier for each spectroscopic object.</li>
    <li><code>class</code>: The class label for each object, which can be one of "STAR", "GALAXY", or "QUASAR".</li>
    <li><code>redshift</code>: A measure of how much the light from the object has been shifted towards the red end of the spectrum due to the expansion of the universe.</li>
    <li><code>plate</code>: The plate number of the spectroscopic observation.</li>
    <li><code>mjd</code>: The modified Julian date of the observation.</li>
    <li><code>fiberid</code>: The fiber ID used in the spectroscopic observation.</li>
</ul>

<h2>Class Labels</h2>
<ul>
    <li><strong>Star</strong>: A luminous spheroid of plasma held together by its own gravity. Stars generate energy through nuclear fusion, with the Sun being the nearest star to Earth.</li>
    <li><strong>Galaxy</strong>: A gravitationally bound system of stars, stellar remnants, interstellar gas, dust, and dark matter. Galaxies can be categorized into different types, such as elliptical, spiral, or irregular.</li>
    <li><strong>Quasar</strong>: Also known as a quasi-stellar object, a quasar is     an extremely luminous active galactic nucleus (AGN). Quasars are among the most powerful objects in the universe, with luminosities exceeding <code>(10<sup>41</sup>)</code> watts, thousands of times greater than an ordinary large galaxy.</li>
</ul>

<h2>Machine Learning Models</h2>

<h3>Random Forest</h3>
<p>Random Forest is an ensemble learning method that constructs multiple decision trees during training and outputs the mode of the classes (classification) of the individual trees. It is robust against overfitting and can handle large datasets with higher dimensionality.</p>

<h4>Key Parameters:</h4>
<ul>
    <li><code>n_estimators</code>: The number of trees in the forest.</li>
    <li><code>max_depth</code>: The maximum depth of the trees.</li>
    <li><code>min_samples_split</code>: The minimum number of samples required to split an internal node.</li>
</ul>

<h3>Support Vector Machine (SVM)</h3>
<p>Support Vector Machine is a supervised learning algorithm that can be used for classification or regression challenges. It works by finding the hyperplane that best separates the classes in the feature space.</p>

<h4>Key Parameters:</h4>
<ul>
    <li><code>C</code>: Regularization parameter that controls the trade-off between achieving a low training error and a low testing error.</li>
    <li><code>kernel</code>: Specifies the kernel type to be used in the algorithm (e.g., linear, polynomial, radial basis function).</li>
    <li><code>gamma</code>: Kernel coefficient for ‘rbf’, ‘poly’, and ‘sigmoid’.</li>
</ul>

<h2>Conclusion</h2>
<p>This analysis aims to classify astronomical objects using machine learning techniques, providing insights into the characteristics of stars, galaxies, and quasars. The results can help in understanding the distribution and properties of these celestial objects in the universe.</p>

<h2>Getting Started</h2>
<p>To run this analysis, ensure you have the following libraries installed:</p>
<ul>
    <li><code>numpy</code></li>
    <li><code>pandas</code></li>
    <li><code>scikit-learn</code></li>
    <li><code>matplotlib</code> (for visualization, if applicable)</li>
</ul>

<p>Clone the repository and run the Jupyter Notebook or Python script to execute the analysis.</p>

<pre><code>git clone &lt;repository-url&gt;
cd &lt;repository-directory&gt;</code></pre>

</body>
</html>
