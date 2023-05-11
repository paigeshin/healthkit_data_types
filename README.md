# healthkit_data_types
```swift

//
//  HKTypeIdentifiers
//  HealthKit
//
//  Copyright (c) 2014-2022 Apple Inc. All rights reserved.
//

/*--------------------------------*/
/*   HKQuantityType Identifiers   */
/*--------------------------------*/

public struct HKQuantityTypeIdentifier : Hashable, Equatable, RawRepresentable, @unchecked Sendable {

    public init(rawValue: String)
}
extension HKQuantityTypeIdentifier {

    
    @available(iOS 8.0, *)
    public static let bodyMassIndex: HKQuantityTypeIdentifier

    @available(iOS 8.0, *)
    public static let bodyFatPercentage: HKQuantityTypeIdentifier // Scalar(Percent, 0.0 - 1.0),  Discrete

    @available(iOS 8.0, *)
    public static let height: HKQuantityTypeIdentifier // Length,                      Discrete

    @available(iOS 8.0, *)
    public static let bodyMass: HKQuantityTypeIdentifier // Mass,                        Discrete

    @available(iOS 8.0, *)
    public static let leanBodyMass: HKQuantityTypeIdentifier // Mass,                        Discrete

    @available(iOS 11.0, *)
    public static let waistCircumference: HKQuantityTypeIdentifier // Length,                      Discrete

    @available(iOS 16.0, *)
    public static let appleSleepingWristTemperature: HKQuantityTypeIdentifier // Temperature,                 Discrete

    
    // Fitness
    @available(iOS 8.0, *)
    public static let stepCount: HKQuantityTypeIdentifier // Scalar(Count),               Cumulative

    @available(iOS 8.0, *)
    public static let distanceWalkingRunning: HKQuantityTypeIdentifier // Length,                      Cumulative

    @available(iOS 8.0, *)
    public static let distanceCycling: HKQuantityTypeIdentifier // Length,                      Cumulative

    @available(iOS 10.0, *)
    public static let distanceWheelchair: HKQuantityTypeIdentifier // Length,                      Cumulative

    @available(iOS 8.0, *)
    public static let basalEnergyBurned: HKQuantityTypeIdentifier // Energy,                      Cumulative

    @available(iOS 8.0, *)
    public static let activeEnergyBurned: HKQuantityTypeIdentifier // Energy,                      Cumulative

    @available(iOS 8.0, *)
    public static let flightsClimbed: HKQuantityTypeIdentifier // Scalar(Count),               Cumulative

    @available(iOS 8.0, *)
    public static let nikeFuel: HKQuantityTypeIdentifier // Scalar(Count),               Cumulative

    @available(iOS 9.3, *)
    public static let appleExerciseTime: HKQuantityTypeIdentifier // Time                         Cumulative

    @available(iOS 10.0, *)
    public static let pushCount: HKQuantityTypeIdentifier // Scalar(Count),               Cumulative

    @available(iOS 10.0, *)
    public static let distanceSwimming: HKQuantityTypeIdentifier // Length,                      Cumulative

    @available(iOS 10.0, *)
    public static let swimmingStrokeCount: HKQuantityTypeIdentifier // Scalar(Count),               Cumulative

    @available(iOS 11.0, *)
    public static let vo2Max: HKQuantityTypeIdentifier // ml/(kg*min)                  Discrete

    @available(iOS 11.2, *)
    public static let distanceDownhillSnowSports: HKQuantityTypeIdentifier // Length,                      Cumulative

    @available(iOS 13.0, *)
    public static let appleStandTime: HKQuantityTypeIdentifier // Time,                        Cumulative

    @available(iOS 14.0, *)
    public static let walkingSpeed: HKQuantityTypeIdentifier // m/s,                         Discrete

    @available(iOS 14.0, *)
    public static let walkingDoubleSupportPercentage: HKQuantityTypeIdentifier // Scalar(Percent, 0.0 - 1.0),  Discrete

    @available(iOS 14.0, *)
    public static let walkingAsymmetryPercentage: HKQuantityTypeIdentifier // Scalar(Percent, 0.0 - 1.0),  Discrete

    @available(iOS 14.0, *)
    public static let walkingStepLength: HKQuantityTypeIdentifier // Length,                      Discrete

    @available(iOS 14.0, *)
    public static let sixMinuteWalkTestDistance: HKQuantityTypeIdentifier // Length,                      Discrete

    @available(iOS 14.0, *)
    public static let stairAscentSpeed: HKQuantityTypeIdentifier // m/s,                         Discrete

    @available(iOS 14.0, *)
    public static let stairDescentSpeed: HKQuantityTypeIdentifier // m/s),                        Discrete

    @available(iOS 14.5, *)
    public static let appleMoveTime: HKQuantityTypeIdentifier // Time,                        Cumulative

    @available(iOS 15.0, *)
    public static let appleWalkingSteadiness: HKQuantityTypeIdentifier // Scalar(Percent, 0.0 - 1.0),  Discrete

    @available(iOS 16.0, *)
    public static let runningStrideLength: HKQuantityTypeIdentifier // Length,                      Discrete

    @available(iOS 16.0, *)
    public static let runningVerticalOscillation: HKQuantityTypeIdentifier // Length,                      Discrete

    @available(iOS 16.0, *)
    public static let runningGroundContactTime: HKQuantityTypeIdentifier // Time,                        Discrete

    @available(iOS 16.0, *)
    public static let runningPower: HKQuantityTypeIdentifier // Power                        Discrete

    @available(iOS 16.0, *)
    public static let runningSpeed: HKQuantityTypeIdentifier // m/s,                         Discrete

    
    // Vitals
    @available(iOS 8.0, *)
    public static let heartRate: HKQuantityTypeIdentifier // Scalar(Count)/Time,          Discrete

    @available(iOS 8.0, *)
    public static let bodyTemperature: HKQuantityTypeIdentifier // Temperature,                 Discrete

    @available(iOS 9.0, *)
    public static let basalBodyTemperature: HKQuantityTypeIdentifier // Basal Body Temperature,      Discrete

    @available(iOS 8.0, *)
    public static let bloodPressureSystolic: HKQuantityTypeIdentifier // Pressure,                    Discrete

    @available(iOS 8.0, *)
    public static let bloodPressureDiastolic: HKQuantityTypeIdentifier // Pressure,                    Discrete

    @available(iOS 8.0, *)
    public static let respiratoryRate: HKQuantityTypeIdentifier // Scalar(Count)/Time,          Discrete

    // Beats per minute estimate of a user's lowest heart rate while at rest
    @available(iOS 11.0, *)
    public static let restingHeartRate: HKQuantityTypeIdentifier // Scalar(Count)/Time,          Discrete

    // Average heartbeats per minute captured by an Apple Watch while a user is walking
    @available(iOS 11.0, *)
    public static let walkingHeartRateAverage: HKQuantityTypeIdentifier // Scalar(Count)/Time,          Discrete

    // The standard deviation of heart beat-to-beat intervals (Standard Deviation of Normal to Normal)
    @available(iOS 11.0, *)
    public static let heartRateVariabilitySDNN: HKQuantityTypeIdentifier // Time (ms),                   Discrete

    // The decrease in heart rate from the rate at peak exercise to the rate 1 minute after the cessation of exercise. Always a positive value.
    @available(iOS 16.0, *)
    public static let heartRateRecoveryOneMinute: HKQuantityTypeIdentifier // Scalar(Count)/Time,          Discrete

    
    // Results
    @available(iOS 8.0, *)
    public static let oxygenSaturation: HKQuantityTypeIdentifier // Scalar(Percent, 0.0 - 1.0),  Discrete

    @available(iOS 8.0, *)
    public static let peripheralPerfusionIndex: HKQuantityTypeIdentifier // Scalar(Percent, 0.0 - 1.0),  Discrete

    @available(iOS 8.0, *)
    public static let bloodGlucose: HKQuantityTypeIdentifier // Mass/Volume,                 Discrete

    @available(iOS 8.0, *)
    public static let numberOfTimesFallen: HKQuantityTypeIdentifier // Scalar(Count),               Cumulative

    @available(iOS 8.0, *)
    public static let electrodermalActivity: HKQuantityTypeIdentifier // Conductance,                 Discrete

    @available(iOS 8.0, *)
    public static let inhalerUsage: HKQuantityTypeIdentifier // Scalar(Count),               Cumulative

    @available(iOS 11.0, *)
    public static let insulinDelivery: HKQuantityTypeIdentifier // Pharmacology (IU)            Cumulative

    @available(iOS 8.0, *)
    public static let bloodAlcoholContent: HKQuantityTypeIdentifier // Scalar(Percent, 0.0 - 1.0),  Discrete

    @available(iOS 8.0, *)
    public static let forcedVitalCapacity: HKQuantityTypeIdentifier // Volume,                      Discrete

    @available(iOS 8.0, *)
    public static let forcedExpiratoryVolume1: HKQuantityTypeIdentifier // Volume,                      Discrete

    @available(iOS 8.0, *)
    public static let peakExpiratoryFlowRate: HKQuantityTypeIdentifier // Volume/Time,                 Discrete

    @available(iOS 13.0, *)
    public static let environmentalAudioExposure: HKQuantityTypeIdentifier // Pressure,                    DiscreteEquivalentContinuousLevel

    @available(iOS 13.0, *)
    public static let headphoneAudioExposure: HKQuantityTypeIdentifier // Pressure,                    DiscreteEquivalentContinuousLevel

    @available(iOS 15.0, *)
    public static let numberOfAlcoholicBeverages: HKQuantityTypeIdentifier // Scalar(Count),               Cumulative

    
    // Nutrition
    @available(iOS 8.0, *)
    public static let dietaryFatTotal: HKQuantityTypeIdentifier // Mass,   Cumulative

    @available(iOS 8.0, *)
    public static let dietaryFatPolyunsaturated: HKQuantityTypeIdentifier // Mass,   Cumulative

    @available(iOS 8.0, *)
    public static let dietaryFatMonounsaturated: HKQuantityTypeIdentifier // Mass,   Cumulative

    @available(iOS 8.0, *)
    public static let dietaryFatSaturated: HKQuantityTypeIdentifier // Mass,   Cumulative

    @available(iOS 8.0, *)
    public static let dietaryCholesterol: HKQuantityTypeIdentifier // Mass,   Cumulative

    @available(iOS 8.0, *)
    public static let dietarySodium: HKQuantityTypeIdentifier // Mass,   Cumulative

    @available(iOS 8.0, *)
    public static let dietaryCarbohydrates: HKQuantityTypeIdentifier // Mass,   Cumulative

    @available(iOS 8.0, *)
    public static let dietaryFiber: HKQuantityTypeIdentifier // Mass,   Cumulative

    @available(iOS 8.0, *)
    public static let dietarySugar: HKQuantityTypeIdentifier // Mass,   Cumulative

    @available(iOS 8.0, *)
    public static let dietaryEnergyConsumed: HKQuantityTypeIdentifier // Energy, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryProtein: HKQuantityTypeIdentifier // Mass,   Cumulative

    
    @available(iOS 8.0, *)
    public static let dietaryVitaminA: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryVitaminB6: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryVitaminB12: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryVitaminC: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryVitaminD: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryVitaminE: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryVitaminK: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryCalcium: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryIron: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryThiamin: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryRiboflavin: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryNiacin: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryFolate: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryBiotin: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryPantothenicAcid: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryPhosphorus: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryIodine: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryMagnesium: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryZinc: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietarySelenium: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryCopper: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryManganese: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryChromium: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryMolybdenum: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryChloride: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryPotassium: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 8.0, *)
    public static let dietaryCaffeine: HKQuantityTypeIdentifier // Mass, Cumulative

    @available(iOS 9.0, *)
    public static let dietaryWater: HKQuantityTypeIdentifier // Volume, Cumulative

    
    @available(iOS 9.0, *)
    public static let uvExposure: HKQuantityTypeIdentifier // Scalar(Count), Discrete

    
    @available(iOS 16.0, *)
    public static let atrialFibrillationBurden: HKQuantityTypeIdentifier // Scalar(Percent, 0.0 - 1.0),  Discrete

    
    @available(iOS 16.0, *)
    public static let underwaterDepth: HKQuantityTypeIdentifier // Length, Discrete

    @available(iOS 16.0, *)
    public static let waterTemperature: HKQuantityTypeIdentifier // Temperature, Discrete
}

/*--------------------------------*/
/*   HKCategoryType Identifiers   */
/*--------------------------------*/

public struct HKCategoryTypeIdentifier : Hashable, Equatable, RawRepresentable, @unchecked Sendable {

    public init(rawValue: String)
}
extension HKCategoryTypeIdentifier {

    
    @available(iOS 8.0, *)
    public static let sleepAnalysis: HKCategoryTypeIdentifier

    @available(iOS 9.0, *)
    public static let appleStandHour: HKCategoryTypeIdentifier // HKCategoryValueAppleStandHour

    @available(iOS 9.0, *)
    public static let cervicalMucusQuality: HKCategoryTypeIdentifier // HKCategoryValueCervicalMucusQuality

    @available(iOS 9.0, *)
    public static let ovulationTestResult: HKCategoryTypeIdentifier // HKCategoryValueOvulationTestResult

    @available(iOS 15.0, *)
    public static let pregnancyTestResult: HKCategoryTypeIdentifier // HKCategoryValuePregnancyTestResult

    @available(iOS 15.0, *)
    public static let progesteroneTestResult: HKCategoryTypeIdentifier // HKCategoryValueProgesteroneTestResult

    @available(iOS 9.0, *)
    public static let menstrualFlow: HKCategoryTypeIdentifier // HKCategoryValueMenstrualFlow

    @available(iOS 9.0, *)
    public static let intermenstrualBleeding: HKCategoryTypeIdentifier // (Spotting) HKCategoryValue

    @available(iOS 16.0, *)
    public static let persistentIntermenstrualBleeding: HKCategoryTypeIdentifier // HKCategoryValue

    @available(iOS 16.0, *)
    public static let prolongedMenstrualPeriods: HKCategoryTypeIdentifier // HKCategoryValue

    @available(iOS 16.0, *)
    public static let irregularMenstrualCycles: HKCategoryTypeIdentifier // HKCategoryValue

    @available(iOS 16.0, *)
    public static let infrequentMenstrualCycles: HKCategoryTypeIdentifier // HKCategoryValue

    @available(iOS 9.0, *)
    public static let sexualActivity: HKCategoryTypeIdentifier // HKCategoryValue

    @available(iOS 10.0, *)
    public static let mindfulSession: HKCategoryTypeIdentifier // HKCategoryValue

    @available(iOS 12.2, *)
    public static let highHeartRateEvent: HKCategoryTypeIdentifier // HKCategoryValue

    @available(iOS 12.2, *)
    public static let lowHeartRateEvent: HKCategoryTypeIdentifier // HKCategoryValue

    @available(iOS 12.2, *)
    public static let irregularHeartRhythmEvent: HKCategoryTypeIdentifier // HKCategoryValue

    @available(iOS, introduced: 13.0, deprecated: 14.0, renamed: "HKCategoryTypeIdentifier.environmentalAudioExposureEvent")
    public static let audioExposureEvent: HKCategoryTypeIdentifier // HKCategoryValueAudioExposureEvent

    
    @available(iOS 13.0, *)
    public static let toothbrushingEvent: HKCategoryTypeIdentifier // HKCategoryValue

    @available(iOS 14.3, *)
    public static let pregnancy: HKCategoryTypeIdentifier // HKCategoryValue

    @available(iOS 14.3, *)
    public static let lactation: HKCategoryTypeIdentifier // HKCategoryValue

    @available(iOS 14.3, *)
    public static let contraceptive: HKCategoryTypeIdentifier // HKCategoryValueContraceptive

    @available(iOS 14.0, *)
    public static let environmentalAudioExposureEvent: HKCategoryTypeIdentifier // HKCategoryValueEnvironmentalAudioExposureEvent

    @available(iOS 14.2, *)
    public static let headphoneAudioExposureEvent: HKCategoryTypeIdentifier // HKCategoryValueHeadphoneAudioExposureEvent

    @available(iOS 14.0, *)
    public static let handwashingEvent: HKCategoryTypeIdentifier // HKCategoryValue

    @available(iOS 14.3, *)
    public static let lowCardioFitnessEvent: HKCategoryTypeIdentifier

    @available(iOS 15.0, *)
    public static let appleWalkingSteadinessEvent: HKCategoryTypeIdentifier // HKCategoryValueAppleWalkingSteadinessEvent

    
    // Symptoms
    @available(iOS 13.6, *)
    public static let abdominalCramps: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let acne: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let appetiteChanges: HKCategoryTypeIdentifier // HKCategoryValueAppetiteChanges

    @available(iOS 14.0, *)
    public static let bladderIncontinence: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let bloating: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let breastPain: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let chestTightnessOrPain: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let chills: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let constipation: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let coughing: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let diarrhea: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let dizziness: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 14.0, *)
    public static let drySkin: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let fainting: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let fatigue: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let fever: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let generalizedBodyAche: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 14.0, *)
    public static let hairLoss: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let headache: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let heartburn: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let hotFlashes: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let lossOfSmell: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let lossOfTaste: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let lowerBackPain: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 14.0, *)
    public static let memoryLapse: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let moodChanges: HKCategoryTypeIdentifier // HKCategoryValuePresence

    @available(iOS 13.6, *)
    public static let nausea: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 14.0, *)
    public static let nightSweats: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let pelvicPain: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let rapidPoundingOrFlutteringHeartbeat: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let runnyNose: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let shortnessOfBreath: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let sinusCongestion: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let skippedHeartbeat: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let sleepChanges: HKCategoryTypeIdentifier // HKCategoryValuePresence

    @available(iOS 13.6, *)
    public static let soreThroat: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 14.0, *)
    public static let vaginalDryness: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let vomiting: HKCategoryTypeIdentifier // HKCategoryValueSeverity

    @available(iOS 13.6, *)
    public static let wheezing: HKCategoryTypeIdentifier // HKCategoryValueSeverity
}

/*--------------------------------------*/
/*   HKCharacteristicType Identifiers   */
/*--------------------------------------*/

public struct HKCharacteristicTypeIdentifier : Hashable, Equatable, RawRepresentable, @unchecked Sendable {

    public init(rawValue: String)
}
extension HKCharacteristicTypeIdentifier {

    
    @available(iOS 8.0, *)
    public static let biologicalSex: HKCharacteristicTypeIdentifier

    @available(iOS 8.0, *)
    public static let bloodType: HKCharacteristicTypeIdentifier // HKBloodTypeObject

    @available(iOS 8.0, *)
    public static let dateOfBirth: HKCharacteristicTypeIdentifier // NSDateComponents

    @available(iOS 9.0, *)
    public static let fitzpatrickSkinType: HKCharacteristicTypeIdentifier // HKFitzpatrickSkinTypeObject

    @available(iOS 10.0, *)
    public static let wheelchairUse: HKCharacteristicTypeIdentifier // HKWheelchairUseObject

    @available(iOS 14.0, *)
    public static let activityMoveMode: HKCharacteristicTypeIdentifier // HKActivityMoveModeObject
}

/*-----------------------------------*/
/*   HKCorrelationType Identifiers   */
/*-----------------------------------*/

public struct HKCorrelationTypeIdentifier : Hashable, Equatable, RawRepresentable, @unchecked Sendable {

    public init(rawValue: String)
}
extension HKCorrelationTypeIdentifier {

    
    @available(iOS 8.0, *)
    public static let bloodPressure: HKCorrelationTypeIdentifier

    @available(iOS 8.0, *)
    public static let food: HKCorrelationTypeIdentifier
}

/*--------------------------------*/
/*   HKDocumentType Identifiers   */
/*--------------------------------*/

public struct HKDocumentTypeIdentifier : Hashable, Equatable, RawRepresentable, @unchecked Sendable {

    public init(rawValue: String)
}
extension HKDocumentTypeIdentifier {

    
    @available(iOS 10.0, *)
    public static let CDA: HKDocumentTypeIdentifier
}

/*------------------------------*/
/*   HKWorkoutType Identifier   */
/*------------------------------*/

@available(iOS 8.0, *)
public let HKWorkoutTypeIdentifier: String

/*--------------------------------*/
/*   HKSeriesSample Identifiers   */
/*--------------------------------*/

@available(iOS 11.0, *)
public let HKWorkoutRouteTypeIdentifier: String
@available(iOS 13.0, *)
public let HKDataTypeIdentifierHeartbeatSeries: String

/*-----------------------------------*/
/* HKVisionPrescription Identifier   */
/*-----------------------------------*/

@available(iOS 16.0, *)
public let HKVisionPrescriptionTypeIdentifier: String

```

```swift
/*--------------------------------*/
/*   HKQuantityType Identifiers   */
/*--------------------------------*/

// Body Measurements
HK_EXTERN NSString * const HKQuantityTypeIdentifierBodyMassIndex NS_AVAILABLE_IOS(8_0);             // Scalar(Count),               Discrete
HK_EXTERN NSString * const HKQuantityTypeIdentifierBodyFatPercentage NS_AVAILABLE_IOS(8_0);         // Scalar(Percent, 0.0 - 1.0),  Discrete
HK_EXTERN NSString * const HKQuantityTypeIdentifierHeight NS_AVAILABLE_IOS(8_0);                    // Length,                      Discrete
HK_EXTERN NSString * const HKQuantityTypeIdentifierBodyMass NS_AVAILABLE_IOS(8_0);                  // Mass,                        Discrete
HK_EXTERN NSString * const HKQuantityTypeIdentifierLeanBodyMass NS_AVAILABLE_IOS(8_0);              // Mass,                        Discrete

// Fitness
HK_EXTERN NSString * const HKQuantityTypeIdentifierStepCount NS_AVAILABLE_IOS(8_0);                 // Scalar(Count),               Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDistanceWalkingRunning NS_AVAILABLE_IOS(8_0);    // Length,                      Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDistanceCycling NS_AVAILABLE_IOS(8_0);           // Length,                      Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierBasalEnergyBurned NS_AVAILABLE_IOS(8_0);         // Energy,                      Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierActiveEnergyBurned NS_AVAILABLE_IOS(8_0);        // Energy,                      Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierFlightsClimbed NS_AVAILABLE_IOS(8_0);            // Scalar(Count),               Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierNikeFuel NS_AVAILABLE_IOS(8_0);                  // Scalar(Count),               Cumulative

// Vitals
HK_EXTERN NSString * const HKQuantityTypeIdentifierHeartRate NS_AVAILABLE_IOS(8_0);                 // Scalar(Count)/Time,          Discrete
HK_EXTERN NSString * const HKQuantityTypeIdentifierBodyTemperature NS_AVAILABLE_IOS(8_0);           // Temperature,                 Discrete
HK_EXTERN NSString * const HKQuantityTypeIdentifierBasalBodyTemperature NS_AVAILABLE_IOS(9_0);      // Basal Body Temperature,      Discrete
HK_EXTERN NSString * const HKQuantityTypeIdentifierBloodPressureSystolic NS_AVAILABLE_IOS(8_0);     // Pressure,                    Discrete
HK_EXTERN NSString * const HKQuantityTypeIdentifierBloodPressureDiastolic NS_AVAILABLE_IOS(8_0);    // Pressure,                    Discrete
HK_EXTERN NSString * const HKQuantityTypeIdentifierRespiratoryRate NS_AVAILABLE_IOS(8_0);           // Scalar(Count)/Time,          Discrete

// Results
HK_EXTERN NSString * const HKQuantityTypeIdentifierOxygenSaturation NS_AVAILABLE_IOS(8_0);          // Scalar (Percent, 0.0 - 1.0,  Discrete
HK_EXTERN NSString * const HKQuantityTypeIdentifierPeripheralPerfusionIndex NS_AVAILABLE_IOS(8_0);  // Scalar(Percent, 0.0 - 1.0),  Discrete
HK_EXTERN NSString * const HKQuantityTypeIdentifierBloodGlucose NS_AVAILABLE_IOS(8_0);              // Mass/Volume,                 Discrete
HK_EXTERN NSString * const HKQuantityTypeIdentifierNumberOfTimesFallen NS_AVAILABLE_IOS(8_0);       // Scalar(Count),               Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierElectrodermalActivity NS_AVAILABLE_IOS(8_0);     // Conductance,                 Discrete
HK_EXTERN NSString * const HKQuantityTypeIdentifierInhalerUsage NS_AVAILABLE_IOS(8_0);              // Scalar(Count),               Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierBloodAlcoholContent NS_AVAILABLE_IOS(8_0);       // Scalar(Percent, 0.0 - 1.0),  Discrete
HK_EXTERN NSString * const HKQuantityTypeIdentifierForcedVitalCapacity NS_AVAILABLE_IOS(8_0);       // Volume,                      Discrete
HK_EXTERN NSString * const HKQuantityTypeIdentifierForcedExpiratoryVolume1 NS_AVAILABLE_IOS(8_0);   // Volume,                      Discrete
HK_EXTERN NSString * const HKQuantityTypeIdentifierPeakExpiratoryFlowRate NS_AVAILABLE_IOS(8_0);    // Volume/Time,                 Discrete

// Nutrition
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryFatTotal NS_AVAILABLE_IOS(8_0);           // Mass,   Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryFatPolyunsaturated NS_AVAILABLE_IOS(8_0); // Mass,   Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryFatMonounsaturated NS_AVAILABLE_IOS(8_0); // Mass,   Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryFatSaturated NS_AVAILABLE_IOS(8_0);       // Mass,   Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryCholesterol NS_AVAILABLE_IOS(8_0);        // Mass,   Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietarySodium NS_AVAILABLE_IOS(8_0);             // Mass,   Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryCarbohydrates NS_AVAILABLE_IOS(8_0);      // Mass,   Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryFiber NS_AVAILABLE_IOS(8_0);              // Mass,   Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietarySugar NS_AVAILABLE_IOS(8_0);              // Mass,   Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryEnergyConsumed NS_AVAILABLE_IOS(8_0);     // Energy, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryProtein NS_AVAILABLE_IOS(8_0);            // Mass,   Cumulative

HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryVitaminA NS_AVAILABLE_IOS(8_0);           // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryVitaminB6 NS_AVAILABLE_IOS(8_0);          // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryVitaminB12 NS_AVAILABLE_IOS(8_0);         // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryVitaminC NS_AVAILABLE_IOS(8_0);           // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryVitaminD NS_AVAILABLE_IOS(8_0);           // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryVitaminE NS_AVAILABLE_IOS(8_0);           // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryVitaminK NS_AVAILABLE_IOS(8_0);           // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryCalcium NS_AVAILABLE_IOS(8_0);            // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryIron NS_AVAILABLE_IOS(8_0);               // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryThiamin NS_AVAILABLE_IOS(8_0);            // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryRiboflavin NS_AVAILABLE_IOS(8_0);         // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryNiacin NS_AVAILABLE_IOS(8_0);             // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryFolate NS_AVAILABLE_IOS(8_0);             // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryBiotin NS_AVAILABLE_IOS(8_0);             // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryPantothenicAcid NS_AVAILABLE_IOS(8_0);    // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryPhosphorus NS_AVAILABLE_IOS(8_0);         // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryIodine NS_AVAILABLE_IOS(8_0);             // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryMagnesium NS_AVAILABLE_IOS(8_0);          // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryZinc NS_AVAILABLE_IOS(8_0);               // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietarySelenium NS_AVAILABLE_IOS(8_0);           // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryCopper NS_AVAILABLE_IOS(8_0);             // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryManganese NS_AVAILABLE_IOS(8_0);          // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryChromium NS_AVAILABLE_IOS(8_0);           // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryMolybdenum NS_AVAILABLE_IOS(8_0);         // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryChloride NS_AVAILABLE_IOS(8_0);           // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryPotassium NS_AVAILABLE_IOS(8_0);          // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryCaffeine NS_AVAILABLE_IOS(8_0);           // Mass, Cumulative
HK_EXTERN NSString * const HKQuantityTypeIdentifierDietaryWater NS_AVAILABLE_IOS(9_0);              // Volume, Cumulative

HK_EXTERN NSString * const HKQuantityTypeIdentifierUVExposure NS_AVAILABLE_IOS(9_0);                // Scalar (Count), Discrete

/*--------------------------------*/
/*   HKCategoryType Identifiers   */
/*--------------------------------*/

HK_EXTERN NSString * const HKCategoryTypeIdentifierSleepAnalysis NS_AVAILABLE_IOS(8_0);             // HKCategoryValueSleepAnalysis
HK_EXTERN NSString * const HKCategoryTypeIdentifierSedentaryState NS_AVAILABLE_IOS(9_0);            // HKCategoryValueSedentaryState
HK_EXTERN NSString * const HKCategoryTypeIdentifierCervicalMucusQuality NS_AVAILABLE_IOS(9_0);      // HKCategoryValueCervicalMucusQuality
HK_EXTERN NSString * const HKCategoryTypeIdentifierOvulationTestResult NS_AVAILABLE_IOS(9_0);       // HKCategoryValueOvulationTestResult
HK_EXTERN NSString * const HKCategoryTypeIdentifierMenstrualFlow NS_AVAILABLE_IOS(9_0);             // HKCategoryValueMenstrualFlow
HK_EXTERN NSString * const HKCategoryTypeIdentifierVaginalSpotting NS_AVAILABLE_IOS(9_0);           // HKCategoryValue
HK_EXTERN NSString * const HKCategoryTypeIdentifierSexualActivity NS_AVAILABLE_IOS(9_0);            // HKCategoryValue


/*--------------------------------------*/
/*   HKCharacteristicType Identifiers   */
/*--------------------------------------*/

HK_EXTERN NSString * const HKCharacteristicTypeIdentifierBiologicalSex NS_AVAILABLE_IOS(8_0); // NSNumber (HKCharacteristicBiologicalSex)
HK_EXTERN NSString * const HKCharacteristicTypeIdentifierBloodType NS_AVAILABLE_IOS(8_0);     // NSNumber (HKCharacteristicBloodType)
HK_EXTERN NSString * const HKCharacteristicTypeIdentifierDateOfBirth NS_AVAILABLE_IOS(8_0);   // NSDate
HK_EXTERN NSString * const HKCharacteristicTypeIdentifierFitzpatrickSkinType NS_AVAILABLE_IOS(9_0); // HKFitzpatrickSkinType

/*-----------------------------------*/
/*   HKCorrelationType Identifiers   */
/*-----------------------------------*/

HK_EXTERN NSString * const HKCorrelationTypeIdentifierBloodPressure NS_AVAILABLE_IOS(8_0);
HK_EXTERN NSString * const HKCorrelationTypeIdentifierFood NS_AVAILABLE_IOS(8_0);

/*------------------------------*/
/*   HKWorkoutType Identifier   */
/*------------------------------*/

HK_EXTERN NSString * const HKWorkoutTypeIdentifier NS_AVAILABLE_IOS(8_0);

```
