# DataWeaver

Visual ETL pipeline builder with AI-suggested transformations.

## Overview

DataWeaver is a no-code data pipeline designer with intelligent transformation suggestions. It connects to 50+ data sources, previews data at each pipeline step, and auto-generates documentation for your workflows.

## Features

- **Visual Pipeline Builder**: Drag-and-drop interface for constructing data flows
- **AI Suggestions**: Intelligent recommendations for data transformations
- **Live Data Preview**: See data transformations in real-time at each step
- **50+ Connectors**: Pre-built connections to databases, APIs, and file formats
- **Auto Documentation**: Generate pipeline documentation automatically
- **Version Control**: Track changes to pipeline configurations

## Technical Stack

- **TypeScript** - Type-safe pipeline definitions
- **Apache Spark** - Distributed data processing engine
- **OpenAI** - Intelligent transformation suggestions
- **React Flow** - Visual node-based editor
- **PostgreSQL** - Metadata and configuration storage

## Pipeline Architecture

```
┌─────────────────────────────────────────────────────┐
│                 DataWeaver Canvas                    │
│                                                      │
│  ┌──────┐    ┌──────┐    ┌──────┐    ┌──────┐      │
│  │Source│───▶│Filter│───▶│ Join │───▶│ Sink │      │
│  │ Node │    │ Node │    │ Node │    │ Node │      │
│  └──────┘    └──────┘    └──────┘    └──────┘      │
│                                                      │
└─────────────────────────────────────────────────────┘
                        │
                        ▼
┌─────────────────────────────────────────────────────┐
│              Spark Execution Engine                  │
│  ┌─────────────────────────────────────────────┐   │
│  │ DAG Optimization → Task Distribution → Run  │   │
│  └─────────────────────────────────────────────┘   │
└─────────────────────────────────────────────────────┘
```

## Supported Sources

**Databases**: PostgreSQL, MySQL, MongoDB, Snowflake, BigQuery
**Cloud Storage**: S3, GCS, Azure Blob
**APIs**: REST, GraphQL, Salesforce, HubSpot
**Files**: CSV, JSON, Parquet, Excel, XML

## Transformation Types

- Filter & Selection
- Aggregation & Grouping
- Join & Merge
- Pivot & Unpivot
- Type Casting
- Deduplication
- Custom Expressions

## Demo

View the live demo at: https://danielminton.github.io/DataWeaver/

## Local Development

```bash
npm install
npm run dev
```

## Author

Daniel Minton