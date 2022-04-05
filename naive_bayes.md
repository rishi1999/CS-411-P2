# README for Problem \#2: Naive Bayes

### safe_log(x)
Returns `-inf` if `x=0` and `log(x)` otherwise.

### read_train(filename)
Reads training data from file `filename` and updates counts for each class-attribute pair.

### smoothed(smoothing, amt, val)
Helper function for smoothing of zero-count values. If `smoothing` is `False`, then returns `val`. Else, returns `val + amt`.

### model_str(n, attr_vars, class_var, class_attr_counts, class_counts, attr_domains, class_domain, smoothing)
Returns a string representation of the trained Naive Bayes model to be printed as required in the assignment.

### classify(file_in, file_out, n, class_attr_counts, class_counts, attr_domains, class_domain, smoothing)
Reads testing data file `file_in`, classifies testing data, and writes results to file `file_out`.