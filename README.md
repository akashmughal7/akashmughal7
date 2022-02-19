import SoftwareDeveloper from 'akash'; 
import { Languages, Frameworks } from 'akash/skills';

class Bio extends SoftwareDeveloper {
  name     = 'Akash Ali';
  title    = 'Senior Software Developer';
  location = 'Lahore,Punjab,Pakistan';
}

class Skills extends SoftwareDeveloper {
  languages  = ['JavaScript', 'PHP'];
  databases  = ['MySQL', 'MongoDB'];
  frameworks = ['Bootstrap', 'Laravel'];
}



