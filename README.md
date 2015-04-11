# SolarImpulse2
"Componentize the Web": Re-implementation of Si2 HB-SIB 's Cockpit as a 
declarative Single Page Web App in Polymer using Web Components.

## Implementation

### Client Side
- HTML5
- Custom Elements flightPanel-* implemented in Polymer
- Polymer Designer for prototyping and layout
- loads Polyfills for older Web browsers that do not yet support Web Components, etc
- Angular 2.0 for glue and user interaction (planned)

### Server Side
- NodeJS as application server
- Server-Side Events (SSE) for light-weight, uni-directional server to clients
  signaling
- REST API to memcached server of SolarImpulse to get telementry in near real-time
- Reverse Proxy with node-http-proxy as Application Level Gateway and SSL engine
- OpenBSD as server platform
