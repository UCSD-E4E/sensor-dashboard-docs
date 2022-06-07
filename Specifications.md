# E4E Sensor Dashboard
## Generic Dashboard for Sensor Health

**Initial Pilot**: San Diego Zoo

### Basic Application Requirements
#### 0. Common Requriements
1. Must be able to be run without being connected to the internet
2. Must use https with either provided certificate or self-signed

#### 1. Front End User Interface
1. Configurable dashboard which is able to pull data from multiple sources
2. Handle different displays for the following data types:
* Numeric
* Video
* Audio
3. Displays include the following:
* Video/audio player
* Line graph
* Bar graph
* Gauge graph
4. Requires log in to view dashboard
5. User cannot join without invitation
6. Front End uses REST API

#### 2. REST API
1. There exists authenticated CRUD API for 
2. Python API wrapper around REST API

#### 3. Administrative Back End
1. Different levels of user rights
2. Ability to send user invitation
3. Add sensors to dashboard
4. Ability to create API keys
5. Leverages REST API

#### 4. Backend Requriements
1. Self contained database/hosted database
2. ARM and x86 compatible
3. Supports templates for how to read from sensors
4. Templates indicate unhealthy condition
5. Support different database backends
6. Store sensor metadata

#### 5. Alerting Requirements
1. Send alerts when sensors are unhealthy when connected to the internet
2. Alerts should be pluggable

### Proposed Software Stack
1. React Front End
2. Ionic/Capacitor/React Native
3. Node backend
4. Unknown datastorage, propose starting with Sqlite


Official Github pages:

See readme's for getting started, Wiki's for in depth descriptions.

https://github.com/UCSD-E4E/sdzwa-sensor-dashboard-backend

https://github.com/UCSD-E4E/sdzwa-sensor-dashboard-frontend
