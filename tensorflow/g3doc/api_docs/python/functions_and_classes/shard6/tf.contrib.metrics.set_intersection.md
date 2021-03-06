### `tf.contrib.metrics.set_intersection(a, b, validate_indices=True)` {#set_intersection}

Compute set intersection of elements in last dimension of `a` and `b`.

All but the last dimension of `a` and `b` must match.

##### Args:


*  <b>`a`</b>: `Output` or `SparseTensor` of the same type as `b`. If sparse, indices
      must be sorted in row-major order.
*  <b>`b`</b>: `Output` or `SparseTensor` of the same type as `a`. Must be
      `SparseTensor` if `a` is `SparseTensor`. If sparse, indices must be
      sorted in row-major order.
*  <b>`validate_indices`</b>: Whether to validate the order and range of sparse indices
     in `a` and `b`.

##### Returns:

  A `SparseTensor` with the same rank as `a` and `b`, and all but the last
  dimension the same. Elements along the last dimension contain the
  intersections.

