# Prioritizating Ceres Components
We’re using a scored prioritization framework for products (features) to help determine our development roadmap.

This is not in contrast to the success spectrum earlier developed, but helps support our team in implementation of our development plans in a manner that will drive the most value to users while the solution is being developed, while making the best use of resources.


## Framework
The scoring framework is found below. All metrics are scored on a scale of 0 - 3. An exception is made for dependencies - where the scoring metric scale is 0, 1, 2 and 10.

<table style="width:100%">
  <tr>
   <td></td>
   <td><strong>0</strong></td>
   <td><strong>1</strong></td>
   <td><strong>2</strong></td>
   <td><strong>3</strong></td>
  </tr>
  <tr>
   <td>Impact</td>
   <td>No impact</td>
   <td>Some impact</td>
   <td>Significant impact</td>
   <td>Radical impact</td>
  </tr>
  <tr>
   <td>Users</td>
   <td>No users</td>
   <td>Less than 30%</td>
   <td>Btw 30 & 70%</td>
   <td>Over 70%</td>
  </tr>
  <tr>
   <td>Dependent Apps</td>
   <td>No apps</td>
   <td>Only 1 app</td>
   <td>>=2 apps</td>
   <td>All apps 
   (score of 10 assigned)</td>
  </tr>
  <tr>
   <td>Cost</td>
   <td>Significant cost</td>
   <td>Some cost</td>
   <td>Low cost</td>
   <td>No cost</td>
  </tr>
</table>

## Scoring the Priorities
<table>
  <tr>
   <td></td>
   <td><strong>Entry Tool</strong></td>
   <td><strong>Upload Tool</strong></td>
   <td><strong>External Tool</strong></td>
   <td><strong>Analysis Tool</strong></td>
   <td><strong>Storage Tool</strong></td>
  </tr>
  <tr>
   <td>
      <strong>Impact</strong><br>
      How impactful would this be in respect to delivering on our vision of reducing time spent generating insights?
   </td>
   <td>3</td>
   <td>3</td>
   <td>2</td>
   <td>1</td>
   <td>3</td>
  </tr>
  <tr>
   <td><strong>Users</strong><br>
   What portion of our users would likely go ahead and use this tool immediately after it launched?
   </td>
   <td>2</td>
   <td>2</td>
   <td>3</td>
   <td>2</td>
   <td>3</td>
  </tr>
  <tr>
   <td>
      <strong>Dependency</strong><br>
      How much do other tools require this tool to be built to work? 
   </td>
   <td>1</td>
   <td>1</td>
   <td>1</td>
   <td>0</td>
   <td>10</td>
  </tr>
  <tr>
   <td>
      <strong>Cost</strong><br>
      What is the cost to deliver this? Cost includes man-hours as a proxy for difficulty and effort
   </td>
   <td>0</td>
   <td>1</td>
   <td>2</td>
   <td>1</td>
   <td>0</td>
  </tr>
  <tr>
   <td><strong>Total</strong></td>
   <td><strong>6</strong></td>
   <td><strong>7</strong></td>
   <td><strong>8</strong></td>
   <td><strong>4</strong></td>
   <td><strong>16</strong></td>
  </tr>
</table>

## Results
Based on this, our order of development would be:
1. Storage tool
2. External data tool
3. Upload tool
4. Entry and Analysis tools

**For this project, we focused on building the alpha prototype of the storage tool, and hope that future development will build out the other components of the Ceres service.**