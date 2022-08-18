# Practicing reprex

library(tidyverse)
library(palmerpenguins)

### NOT A REPREX
penguins %>%
  select(species, body_mass_g, flipper_length_mm, year) %>%
  filter(species == "Chinstrap") %>%
  str_to_lower(species) %>%
  group_by(island) %>%
  summarize(mean(body_mass_g, na.rm = TRUE),
            mean(flipper_length_mm, na.rm = TRUE))

### A REPREX
library(tidyverse) # or library(stringr)

warpbreaks %>%
  str_to_lower(wool)

library(tidyverse)

warpbreaks |>
  str_to_lower(wool)

### A FIXING REPREX

library(tidyverse)

warpbreaks %>% 
  mutate(wool = str_to_lower(wool))

### A REPREX WITH A SYNTHESIZED DATA FRAME
library(tidyverse)

df <- tribble(
  ~sample_column,
  "A",
  "B",
  "C"
)

df %>% 
  mutate(sample_column = str_to_lower(sample_column))