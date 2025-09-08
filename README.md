# 🚗 Automotive Repair Labour Hour Checker

A comprehensive cross-platform mobile app for automotive repair shops to manage VIN decoding, labor calculations, tire pricing, work orders, and unit conversions. Built with React Native and Expo for iOS, Android, and web platforms.

## Features

### 🚗 VIN Decoder
- Decode 17-character VINs to get vehicle information
- Camera scanning capability (mobile only)
- Customer information management
- Sample VINs for testing

### ⏰ Labor Guide
- Look up labor hours for specific repair jobs
- Vehicle-specific labor time calculations
- Comprehensive repair categories
- Professional labor rate calculations

### 🧮 Calculator
- Basic calculator functionality
- Professional design for quick calculations
- Mobile-optimized interface

### 📋 Work Order
- Create and manage work orders
- Add labor items with hours and rates
- Parts cost tracking
- Tax calculations (16% built-in)
- Generate professional quotes
- Save and retrieve work orders

### 🛞 Tire Calculator
- Calculate tire costs per tire
- Tax included in calculations
- Professional pricing interface

### 🔄 Unit Converter
- Convert between various units
- Length, weight, temperature, volume, and more
- Accurate conversion calculations
- Professional interface

## Installation

### Prerequisites
- Node.js (v18 or higher)
- Bun package manager
- Expo CLI
- iOS/Android device or simulator

### Quick Start

1. **Clone the repository:**
```bash
git clone https://github.com/yourusername/automotive-repair-labour-hour-checker.git
cd automotive-repair-labour-hour-checker
```

2. **Install dependencies:**
```bash
# Using npm
npm install

# Using yarn
yarn install

# Using bun (if available)
bun install
```

3. **Start the development server:**
```bash
# Start with Expo
npx expo start

# Or with tunnel for external devices
npx expo start --tunnel

# For web development
npx expo start --web
```

### Running on Mobile Device

1. Install Expo Go app on your iOS/Android device
2. Scan the QR code displayed in the terminal
3. The app will load on your device

## Project Structure

```
app/
├── (tabs)/
│   ├── _layout.tsx          # Tab navigation layout
│   ├── index.tsx            # VIN Decoder screen
│   ├── labor-guide.tsx      # Labor hours lookup
│   ├── calculator.tsx       # Basic calculator
│   ├── work-order.tsx       # Work order management
│   ├── tire-calculator.tsx  # Tire pricing calculator
│   └── unit-converter.tsx   # Unit conversion tool
├── _layout.tsx              # Root layout
hooks/
├── vehicle-store.ts         # Global state management
types/
├── vehicle.ts              # TypeScript type definitions
utils/
├── vin-decoder.ts          # VIN decoding logic
├── labor-calculator.ts     # Labor calculations
└── responsive.ts           # Responsive design utilities
data/
├── labor-hours.ts          # Labor time database
```

## Key Technologies

- **React Native**: Cross-platform mobile development
- **Expo**: Development platform and tools
- **TypeScript**: Type-safe JavaScript
- **Expo Router**: File-based navigation
- **AsyncStorage**: Local data persistence
- **React Query**: Server state management
- **Lucide Icons**: Beautiful icon library

## Configuration

### App Configuration (app.json)
- App name: "Automotive Repair Labour Hour Checker"
- Bundle ID: `app.rork.automotive-repair-labour-hour-checker`
- Supports tablets and phones
- Camera permissions configured

### Features
- **Cross-platform**: Works on iOS, Android, and web
- **Offline capable**: Data stored locally
- **Professional UI**: Dark theme with orange accents
- **Mobile-optimized**: Touch-friendly interface
- **Type-safe**: Full TypeScript implementation

## Sample Data

The app includes sample VINs for testing:
- `1HGBH41JXMN109186` - 2021 Honda Civic
- `5YJSA1E26HF176643` - 2017 Tesla Model S
- `WBA8E9G59GNT78911` - 2016 BMW 3 Series
- `1FTFW1ET5DFC10312` - 2013 Ford F-150

## Development

### Available Scripts

- `npm start` - Start Expo development server
- `npm run start:tunnel` - Start with tunnel for external access
- `npm run start:web` - Start web development server
- `npm run android` - Start Android development
- `npm run ios` - Start iOS development
- `npm run lint` - Run ESLint
- `npm test` - Run tests (placeholder)

### Building for Production

This app is configured for Expo Go development. For production builds:

1. **Install EAS CLI:**
```bash
npm install -g @expo/eas-cli
```

2. **Configure EAS Build:**
```bash
eas build:configure
```

3. **Build for platforms:**
```bash
# Build for iOS
eas build --platform ios

# Build for Android
eas build --platform android

# Build for both
eas build --platform all
```

## Shop Information

The app is configured for "Happy Tires Automotive Centre":
- Phone: 905-741-3377
- Email: Happytiresinc@gmail.com

To customize for your shop, edit the `shopInfo` object in `hooks/vehicle-store.ts`.

## License

This project is private and proprietary.

## Support

For support or questions, contact the development team.
