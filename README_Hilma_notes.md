# Environment_calibration

# InsetChart - Blood Smear Parasite Prevalence (Microscopy) -- (applies to RDT or others)

1. simulation_coordinator.csv --- prevalence_comparison_diagnostic = "Microscopy"

2. environmental_calibration -> environmental_calibration_common -> analyzers -> analyze.py
---> Add "Blood Smear Parasite Prevalence" in Insetchart 'channels'

3. environmental_calibration -> environmental_calibration_common -> compare_to_data -> calculate_all_scores.py
---> In 'compare_all_age_PCR_prevalence' make prevalence=('Blood Smear Parasite Prevalence', 'mean') 

4. environmental_calibration -> environmental_calibration_common -> compare_to_data -> run_full_comparison.py
---> In plot_allAge_prevalence change plt.plot and plt.ylabel to "Blood Smear Parasite Prevalence"

5. environmental_calibration -> simulations -> output -> 'exp_label' -> 'LF_' -> SO -> 'site name' -> InsetChart
---> Confirm if InsetChart has "Blood Smear Parasite Prevalence"


