
<div>
  <h1>Interactive Image Filter Application</h1>
  
  <h2>Project Overview</h2>
  <p>This web-based application provides real-time image processing capabilities through a browser interface. Unlike traditional desktop applications, this tool requires cloud deployment or a properly configured Python environment to function, as it relies on server-side processing through Gradio's web framework.</p>
  
  <h2>Key Features</h2>
  <div class="features-grid">
    <div class="feature-card">
      <h3>Noise Operations</h3>
      <ul>
        <li>Gaussian Noise Injection</li>
        <li>Salt & Pepper Noise</li>
        <li>Advanced Noise Removal (Non-local Means Denoising)</li>
      </ul>
    </div>
    
   <div class="feature-card">
      <h3>Morphological Processing</h3>
      <ul>
        <li>Erosion with configurable kernels</li>
        <li>Dilation operations</li>
        <li>Opening/Closing for noise removal</li>
      </ul>
    </div>
    
  <div class="feature-card">
      <h3>Thresholding Suite</h3>
      <ul>
        <li>Global Threshold (Manual)</li>
        <li>Adaptive Threshold (Gaussian-weighted)</li>
        <li>Otsu's Automatic Thresholding</li>
      </ul>
    </div>
    
  <div class="feature-card">
      <h3>Advanced CV Techniques</h3>
      <ul>
        <li>Boundary Extraction</li>
        <li>Region Filling Algorithm</li>
        <li>Hough Line Transform</li>
        <li>Watershed Segmentation</li>
        <li>Canny Edge Detection</li>
      </ul>
    </div>
  </div>

  <h2>System Requirements</h2>
  <p><strong>Note:</strong> This is not a standalone desktop application. It requires:</p>
  <ul>
    <li>Python 3.7+ environment</li>
    <li>Web browser for interface</li>
    <li>Server deployment for web access (or localhost operation)</li>
  </ul>

  <h2>Deployment Options</h2>
  <ol>
    <li><strong>Cloud Deployment:</strong>
      <ul>
        <li>Hugging Face Spaces (recommended)</li>
        <li>Google Colab with Gradio share link</li>
        <li>AWS/Azure/GCP with proper Python environment</li>
      </ul>
    </li>
    <li><strong>Local Testing:</strong>
      <ul>
        <li>Requires Python installation with all dependencies</li>
        <li>Accessible only via localhost unless properly forwarded</li>
        <li>Not suitable for end-users without technical setup</li>
      </ul>
    </li>
  </ol>

  <h2>Technical Stack</h2>
  <table>
    <tr>
      <th>Component</th>
      <th>Technology</th>
      <th>Purpose</th>
    </tr>
    <tr>
      <td>Image Processing</td>
      <td>OpenCV 4.x</td>
      <td>Core filter implementations</td>
    </tr>
    <tr>
      <td>Web Interface</td>
      <td>Gradio</td>
      <td>Interactive UI components</td>
    </tr>
    <tr>
      <td>Numerical Operations</td>
      <td>NumPy</td>
      <td>Matrix transformations</td>
    </tr>
    <tr>
      <td>Dependencies</td>
      <td>pip</td>
      <td>Package management</td>
    </tr>
  </table>

<h2>Usage Limitations</h2>
  <ul>
    <li>Requires active Python session to maintain operation</li>
    <li>Image size limitations based on server resources</li>
    <li>No native mobile support (web browser access only)</li>
    <li>Processing speed depends on server capabilities</li>
  </ul>
</div>

<style>
.features-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
  margin: 20px 0;
}
.feature-card {
  border: 1px solid #ddd;
  padding: 15px;
  border-radius: 8px;
}
table {
  border-collapse: collapse;
  width: 100%;
  margin: 20px 0;
}
th, td {
  border: 1px solid #ddd;
  padding: 8px;
  text-align: left;
}
</style>
