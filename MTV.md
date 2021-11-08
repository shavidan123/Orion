# Orion-MTV

This document presents our visualization tool for investigating anomalies in time series data. **MTV** is a visual analytics system built for anomaly analysis of multivariate time-series data.


The visualization platform supports standard operations such as multi-signal viewing and zoom functionalities.
In addition, it allows for a multi-aggregation view, which allows a user to compare the signal at different aggregation levels.
These operations help experts understand why certain intervals have been flagged, and allows for modification and annotation.
In addition, we provide a discussion panel so that team members can comment on or dispute the status of an event.

## Visualization Preview
![Teaser](docs/images/mtv-teaser.png?raw=true "Teaser")

The MTV interface, displaying an analysis of stock data. The Signal Overview (a) displays multiplesignals (in this case, stocks) that share the same horizontal timeline and highlights anomalous events with awarning color (a1). Users pick a signal of interest (i.e., COKE) and brush a segment (a2) to observe its detailsand interact with the events in the Signal Focused View (b). Events can be color-tagged (e.g., green - normal,orange - investigate, red - problem) and filtered in the top header. The predicted errors (b1) can be toggled toexplain why a certain event (b2) was identified by the machine learning algorithm. The Side Panel (c) includesfour collapsible views — the Periodical View (c1, c2), Signal Annotations View, Event Details View, and SimilarSegments View — which allow users to investigate and annotate events efficiently and collaboratively.

## Panel Preview
![Panels](docs/images/mtv-side-panels.png?raw=true "Panels")

Three sub-views in the Side Panel: (a) the Signal Annotation View provides an overview of the annotations (ordered by event time) made for the selected signal; (b) the Event Details View shows moredetails about one particular event, such as severity score and source; (c) the Similar Segments View displaysthe search results of the shape-matching algorithm and allows users to perform quick annotations.