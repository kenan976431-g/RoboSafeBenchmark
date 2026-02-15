# Core API

## robosafe.load_dataset

```python
def load_dataset(split: str, **kwargs) -> Dataset:
    """
    Load dataset.
    
    Args:
        split: Dataset split ("train", "val", "test")
        **kwargs: Additional arguments
    
    Returns:
        Dataset object
    
    Example:
        >>> dataset = robosafe.load_dataset("train")
        >>> print(len(dataset))
        80000
    """
```

## robosafe.train

```python
def train(
    dataset: Dataset, 
    config: Config,
    **kwargs
) -> Model:
    """
    Train a model.
    
    Args:
        dataset: Training dataset
        config: Training configuration
        **kwargs: Additional arguments
    
    Returns:
        Trained model
    """
```

## robosafe.evaluate

```python
def evaluate(
    model: Model,
    dataset: Dataset,
    **kwargs
) -> Dict:
    """
    Evaluate model performance.
    
    Args:
        model: Trained model
        dataset: Evaluation dataset
        **kwargs: Additional arguments
    
    Returns:
        Dictionary of evaluation metrics
    """
```
