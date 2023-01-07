# Text classification notes

![alt text](imgs/spark_text_classification_workflow.png)

imports used:

from pyspark import SparkContext<br>
from pyspark.sql import SparkSession  // To start or create spark session <br>

from pyspark.ml.feature import Tokenizer, StopWordsRemover, CountVectorizer, IDF <br>
from pyspark.ml.feature import StringIndexer // For label encoding/indexing <br>

from pyspark.ml.classification import LogisticRegression <br>
from pyspark.ml import Pipeline // end to end pipeline <br>

from pyspark.ml.evaluation import MulticlassClassificationEvaluator <br>
from pyspark.mllib.evaluation import MulticlassMetrics // Metrics for multiclass classification <br>

from pyspark.sql.types import StringTypes // data type of column/entity <br>
from pyspark.ml.pipline import PipelineModel // To save and load model <br>

from sklearn.metrics import ConfusionMatrixDisplay, confusion_matrix, classification_report // Metric Monitoring

