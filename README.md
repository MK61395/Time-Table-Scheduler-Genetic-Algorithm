# Time-Table-Scheduler-Genetic-Algorithm
A Time Table Scheduler in Python for FAST University Islamabad using Genetic Algorithm.


## Introduction

In the modern academic landscape, efficient timetable scheduling is pivotal for universities to ensure smooth operations and optimal utilization of resources. This project delves into the classical problem of timetable scheduling, aiming to create schedules for each semester with minimal clashes between sections, professors, and rooms. The primary goal is to design a robust algorithmic solution that automates the timetable creation process while adhering to a set of hard and soft constraints.

### Key Challenges

- Ensuring classes are scheduled in available classrooms.
- Accommodating section sizes with appropriate room capacities.
- Avoiding scheduling conflicts for professors and sections.
- Optimizing the allocation of courses to professors and sections.
- Minimizing the number of clashes and interruptions in the timetable.

To tackle these challenges, a genetic algorithm approach is employed, leveraging binary encoding for chromosomes and a fitness function that penalizes clashes and conflicts. The algorithm iteratively refines schedules to achieve optimal solutions that meet the specified constraints.

## Methodology

### Data Preparation and Representation

The project starts by importing necessary libraries such as `Counter` from `collections`, `pandas` for data manipulation, `numpy` for numerical operations, `openpyxl` for Excel file handling, and `random` for generating random numbers. These libraries are essential for data preparation, representation, and algorithm implementation.

### Resource Initialization

For the scheduling of both theory and lab sessions, essential resources such as rooms, labs, lab courses, and lab instructors were initialized. This ensures that the algorithm has access to crucial information for optimizing schedules effectively.

### Genetic Algorithm Parameters

- **Population Size**: 32 chromosomes, representing potential timetable schedules.
- **Number of Generations**: 10,000 generations to refine the schedules.
- **Mutation Probability**: 0.085, determining the likelihood of introducing changes in the chromosomes during evolution.

### Functions Implemented

#### Creating and Cleaning DataFrame

The `create_and_clean_dataframe` function converts Excel data into a structured Pandas DataFrame, adhering to specific constraints based on the sheet name provided. It performs data cleaning operations to ensure the DataFrame is ready for further processing.

#### Mapping Timetable to DataFrame

The `map_timetable_to_dataframe` function maps the generated timetable (represented as a list) to an empty timetable DataFrame. This mapping ensures that the timetable data is structured and organized for easy analysis and manipulation.

#### Binary Encoding of Chromosome Information

The `binary_encode_chromosome` function converts the given chromosome information into binary format, facilitating efficient manipulation and optimization during the timetable scheduling process.

#### Fitness Evaluation Function

The fitness function evaluates the fitness score of a given timetable chromosome based on a set of hard and soft constraints, such as avoiding overlapping classes and meeting room capacity constraints.

#### Selection, Crossover, and Mutation Functions

- **Selection**: Identifies top-performing chromosomes based on their fitness scores.
- **Crossover**: Combines genetic material from two parents to create offspring.
- **Mutation**: Introduces random changes in the offspring chromosomes to maintain diversity in the population.

#### Genetic Algorithm Function

The `genetic_algorithm` function orchestrates the entire genetic algorithm process for timetable scheduling optimization. It iteratively refines the population to improve fitness scores and generate optimal timetable schedules.

### Process Overview

1. **Data Preparation**: Convert and clean Excel data into a structured DataFrame.
2. **Resource Initialization**: Initialize essential resources for scheduling.
3. **Initial Population Generation**: Create an initial population of timetable chromosomes.
4. **Genetic Algorithm Execution**: Evolve the population over multiple generations to optimize schedules.
5. **Fitness Evaluation**: Assess the fitness of the final timetable schedule.

## Results and Analysis

### Genetic Algorithm Execution

The genetic algorithm was executed with the specified parameters and successfully found a chromosome with the maximum possible fitness score, indicating an optimized timetable schedule.

### Fitness Evaluation of Final Timetable

The final timetable achieved a fitness score of 100 out of a maximum possible score of 100, demonstrating excellent adherence to the defined constraints and optimization criteria.

## Conclusion

This project successfully implemented a genetic algorithm to automate the timetable scheduling process, addressing key challenges and achieving optimized schedules for academic institutions. For result and otput, please refer to the attached PDF.

## Contributions

Ahmed Kamal :)

