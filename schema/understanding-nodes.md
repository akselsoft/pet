# Understanding Nodes

In the PET schema, **Understanding Nodes** represent the contextual basis or justification for relationships between nodes. They are not direct links themselves, but rather the explanation or source behind why an edge exists.

## Purpose

Understanding nodes serve as the memory of *why* a connection was made, storing contextual details such as the source, time, and outcome of a learning or observation event.

## Structure

An understanding node typically includes:

- `id`: Unique identifier for the understanding node
- `source`: Entity or context that taught or conveyed the information (e.g., "Father", "Book", "Experience")
- `time`: (optional) Timestamp or reference to when this was learned or formed
- `from`: Originating node ID
- `to`: Target node ID
- `result`: The expected outcome or interpretation (e.g., "exist", "non-exist", "warning", "beneficial")
- `details`: (optional) Any additional description or qualifiers about the context or reliability

## Example
