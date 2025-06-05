
# Edges

In the PET schema, **edges** are the relationships or connections between two or more nodes. These can represent associations such as cause/effect, classification, experience, or sensory correlation.

Unlike traditional edges which are simply directional links (from → to), PET edges may reference an **Understanding Node** that explains the reason or source behind the connection.

## Structure

An edge may include:

- `from`: ID or label of the source node
- `to`: ID or label of the target node
- `type`: (optional) nature of the relationship (e.g., "is-a", "part-of", "experienced-at")
- `understanding_id`: reference to the Understanding Node that justifies this edge
- `weight`: (optional) derived from the neural net to indicate strength or trust
- `existence`: (optional) flag showing whether this edge currently holds in short-term memory

## Example

```
from: Dog  
to: Animal  
type: is-a  
understanding_id: U102  
weight: 0.98  
existence: true
```

## Notes

- Edges can evolve as the neural network adapts to new patterns or reinterpretations.
- Multiple edges between the same pair of nodes may exist, each backed by different understanding nodes.
- The `existence` flag is often calculated by the neural network and represents the current state of belief.
