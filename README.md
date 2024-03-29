# Deepfake Detectiom Benchmark
As increasing deepfake detection methods are proposed, we devote to establish a fair, comprehensive and strict benchmark to quantitatively evaluate these methods considering their in-domain detection ability, cross-domain generalization ability, robustness and practicability. This is an online benchmark in which participating methods would be trained on our standard training datasets(including 7 public datasets) and evaluated on our strandard test datasets and ID test(imperceptible and diverse test) set. The evaluation would be measured by 6 metrics, namely in-domain AUC, cross-domain AUC, AUC vs. perturbation curve, AUC vs. FLOPs curve, AUC vs. number of parameters curve and AUC vs. inference time curve.

As part of the benchmark, we take the lead in re-implementing and evaluating 9 popular detection algorithms from existing literature and publish the leaderboard below. We will maintain the leaderborad of the best detection algorithms as increasing algorithms were incorporated in.

The goal of our benchmark is to offer a comparative and considerable evaluation and further clarify the state-of-the-art among deepfake detection algorithms. Moreover, we hope that our benchmark will serve the deepfake detection community as a standardized benchmark and encourage the researchers to make reproducible and practical contributions to this field.

## Leaderboard on Standard Test Datasets

<table>
    <thead>
        <tr>
          <th>Train</th>
          <th>UADFV</th>
          <th>DF-TIMIT</th>
          <th>Celeb-DF</th>
          <th>DF-1.0</th>
          <th>FF++/DF</th>
          <th>FF++/FS</th>
          <th>FF++/FShifter</th>
          <th>DFDC</th>
          <th>ForgeryNet</th>
          <th rowspan=2>Average AUC(%)</th>
        </tr>
      <tr>
          <th>Test</th>
          <th>UADFV</th>
          <th>DF-TIMIT</th>
          <th>Celeb-DF</th>
          <th>DF-1.0</th>
          <th>FF++/DF</th>
          <th>FF++/FS</th>
          <th>FF++/FShifter</th>
          <th>DFDC</th>
          <th>ForgeryNet</th>
        </tr>
  </thead>
  <tbody>
        <tr>
          <td>Face X-ray</td>
          <td>97.1</td>
          <td>98.5</td>
          <td>97.8</td>
          <td>84.7</td>
          <td>99.4</td>
          <td>99.8</td>
          <td>99.7</td>
          <td>-</td>
          <td>-</td>
          <td>96.7(96.7)</td>
        </tr>
        <tr>
           <td>FWA-Resnet50</td>
           <td>57.3</td>
           <td>99.1</td>
           <td>60.3</td>
           <td>60.5</td>
           <td>80.6</td>
           <td>61.2</td>
           <td>50.0</td>
           <td>47.6</td>
           <td>50.3</td>
           <td>63.6(67.0)</td>
        </tr>
        <tr>
            <td>HeadPose</td>
            <td>88.3</td>
            <td>62.3</td>
            <td>-</td>
            <td>57.2</td>
            <td>57.0</td>
            <td>52.3</td>
            <td>61.2</td>
            <td>-</td>
            <td>-</td>
            <td>63.0(63.0)</td>
        </tr>
        <tr>
            <td>Meosonet-4</td>
            <td>97.7</td>
            <td>100.0</td>
            <td>99.0</td>
            <td>100.0</td>
            <td>99.1</td>
            <td>99.4</td>
            <td>99.6</td>
            <td>93.8</td>
            <td>71.2</td>
            <td>95.5(99.2)</td>
        </tr>
        <tr>
            <td>MeosoIncept-4</td>
            <td>97.8</td>
            <td>100.0</td>
            <td>98.7</td>
            <td>100.0</td>
            <td>98.9</td>
            <td>96.8</td>
            <td>99.5</td>
            <td>94.8</td>
            <td>67.0</td>
            <td>94.8(98.8)</td>
        </tr>
        <tr>
            <td>Patch-resnet</td>
            <td>98.4</td>
            <td>100.0</td>
            <td>89.8</td>
            <td>99.9</td>
            <td>99.5</td>
            <td>99.7</td>
            <td>99.5</td>
            <td>90.1</td>
            <td>60.5</td>
            <td>92.4(98.1)</td>
        </tr>
        <tr>
            <td>Patch-xception</td>
            <td>97.4</td>
            <td>100.0</td>
            <td>90.9</td>
            <td>100.0</td>
            <td>99.9</td>
            <td>99.6</td>
            <td>99.7</td>
            <td>92.7</td>
            <td>60.1</td>
            <td>93.3(98.2)</td>
        </tr>
        <tr>
            <td>Xception</td>
            <td>95.3</td>
            <td>100.0</td>
            <td>84.7</td>
            <td>98.6</td>
            <td>99.3</td>
            <td>98.4</td>
            <td>99.3</td>
            <td>79.7</td>
            <td>64.4</td>
            <td>91.0(96.5)</td>
        </tr>
        <tr>
            <td>FFD</td>
            <td>99.1</td>
            <td>100.0</td>
            <td>99.5</td>
            <td>75.9</td>
            <td>99.7</td>
            <td>99.6</td>
            <td>100.0</td>
            <td>-</td>
            <td>-</td>
            <td>96.2(96.2)</td>
        </tr>
        <tr>
            <td>Multi-attention</td>
            <td>99.0</td>
            <td>100.0</td>
            <td>100.0</td>
            <td>99.9</td>
            <td>99.2</td>
            <td>99.7</td>
            <td>100.0</td>
            <td>99.0</td>
            <td>80.1</td>
            <td>97.4(99.6)</td>
        </tr>
        <tr>
            <td>Conv LSTM</td>
            <td>99.8</td>
            <td>100.0</td>
            <td>91.9</td>
            <td>99.9</td>
            <td>99.9</td>
            <td>98.7</td>
            <td>100.0</td>
            <td>81.4</td>
            <td>64.5</td>
            <td>92.9(98.6)</td>
        </tr>
        <tr>
            <td>LRNet</td>
            <td>86.9</td>
            <td>98.5</td>
            <td>63.0</td>
            <td>92.4</td>
            <td>96.4</td>
            <td>98.2</td>
            <td>89.9</td>
            <td>51.6</td>
            <td>66.7</td>
            <td>82.6(89.3)</td>
        </tr>
    </tbody>
</table>

## Leaderboard on ID Test Datasets
<table>
    <thead>
        <tr>
          <th>Train</th>
          <th>UADFV</th>
          <th>DF-TIMIT</th>
          <th>Celeb-DF</th>
          <th>DF-1.0</th>
          <th>FF++/DF</th>
          <th>FF++/FS</th>
          <th>FF++/FShifter</th>
          <th>DFDC</th>
          <th>ForgeryNet</th>
          <th rowspan=2>Average AUC(%)</th>
        </tr>
      <tr>
          <th>Test</th>
          <th>UADFV</th>
          <th>DF-TIMIT</th>
          <th>Celeb-DF</th>
          <th>DF-1.0</th>
          <th>FF++/DF</th>
          <th>FF++/FS</th>
          <th>FF++/FShifter</th>
          <th>DFDC</th>
          <th>ForgeryNet</th>
        </tr>
  </thead>
  <tbody>
        <tr>
          <td>Face X-ray</td>
          <td>53.9</td>
          <td>52.1</td>
          <td>64.3</td>
          <td>66.4</td>
          <td>54.4</td>
          <td>59.3</td>
          <td>54.9</td>
          <td>-</td>
          <td>-</td>
          <td>57.9(57.9)</td>
        </tr>
        <tr>
           <td>FWA-Resnet50</td>
           <td>54.7</td>
           <td>55.1</td>
           <td>49.9</td>
           <td>54.3</td>
           <td>49.8</td>
           <td>54.3</td>
           <td>50.0</td>
           <td>53.2</td>
           <td>50.0</td>
           <td>52.3(52.5)</td>
        </tr>
        <tr>
            <td>HeadPose</td>
            <td>52.1</td>
            <td>48.3</td>
            <td>-</td>
            <td>50.4</td>
            <td>51.8</td>
            <td>54.0</td>
            <td>50.7</td>
            <td>-</td>
            <td>-</td>
            <td>51.2(51.2)</td>
        </tr>
        <tr>
            <td>Meosonet-4</td>
            <td>57.2</td>
            <td>59.4</td>
            <td>59.9</td>
            <td>47.4</td>
            <td>53.7</td>
            <td>57.6</td>
            <td>48.6</td>
            <td>61.6</td>
            <td>66.5</td>
            <td>56.8(54.8)</td>
        </tr>
        <tr>
            <td>MeosoIncept-4</td>
            <td>60.0</td>
            <td>55.8</td>
            <td>59.6</td>
            <td>48.3</td>
            <td>54.5</td>
            <td>63.0</td>
            <td>49.8</td>
            <td>60.5</td>
            <td>54.7</td>
            <td>56.2(55.8)</td>
        </tr>
        <tr>
            <td>Patch-resnet</td>
            <td>57.1</td>
            <td>55.9</td>
            <td>54.1</td>
            <td>54.5</td>
            <td>60.0</td>
            <td>64.9</td>
            <td>57.7</td>
            <td>59.8</td>
            <td>56.7</td>
            <td>57.8(57.7)</td>
        </tr>
        <tr>
            <td>Patch-xception</td>
            <td>53.3</td>
            <td>53.5</td>
            <td>56.4</td>
            <td>53.2</td>
            <td>60.3</td>
            <td>63.4</td>
            <td>64.0</td>
            <td>52.8</td>
            <td>58.3</td>
            <td>57.2(57.7)</td>
        </tr>
        <tr>
            <td>Xception</td>
            <td>55.9</td>
            <td>61.9</td>
            <td>52.9</td>
            <td>59.8</td>
            <td>61.6</td>
            <td>52.1</td>
            <td>48.0</td>
            <td>56.3</td>
            <td>57.0</td>
            <td>56.1(56.0)</td>
        </tr>
        <tr>
            <td>FFD</td>
            <td>53.9</td>
            <td>63.4</td>
            <td>62.1</td>
            <td>64.3</td>
            <td>57.8</td>
            <td>57.4</td>
            <td>43.5</td>
            <td>-</td>
            <td>-</td>
            <td>57.4(57.4)</td>
        </tr>
        <tr>
            <td>Multi-attention</td>
            <td>52.0</td>
            <td>54.0</td>
            <td>64.1</td>
            <td>59.3</td>
            <td>54.8</td>
            <td>54.5</td>
            <td>57.4</td>
            <td>74.7</td>
            <td>74.5</td>
            <td>60.5(56.5)</td>
        </tr>
        <tr>
            <td>Conv LSTM</td>
            <td>56.3</td>
            <td>57.7</td>
            <td>59.9</td>
            <td>50.0</td>
            <td>62.9</td>
            <td>55.5</td>
            <td>39.9</td>
            <td>52.2</td>
            <td>50.1</td>
            <td>53.8(54.6)</td>
        </tr>
        <tr>
            <td>LRNet</td>
            <td>52.3</td>
            <td>42.0</td>
            <td>55.4</td>
            <td>51.8</td>
            <td>61.3</td>
            <td>56.4</td>
            <td>53.8</td>
            <td>54.0</td>
            <td>61.8</td>
            <td>54.3(53.2)</td>
        </tr>
    </tbody>
</table>
