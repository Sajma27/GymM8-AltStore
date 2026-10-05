# GymM8 Privacy

Updated 5 October 2026. Applies to GymM8's Forerunner 970 companion and Apple Health integration on iPhone.

## Data used and why

The companion receives your workout name, exercise names, sets, weights, repetitions, split side and rest deadlines from GymM8 on your paired iPhone. It uses these to display your workout and apply the set controls you choose.

While recording, it reads heart rate from the watch and records a Strength Training activity. After a successful save, it sends the activity's calories, average and maximum heart rate, and recorded duration to your paired iPhone so GymM8 can show them in your workout summary and history. Unavailable sensor measurements are omitted.

The integration also stores workout identifiers, message revisions, recent command receipts and the selected Garmin device identifier to reconnect and prevent duplicate actions. The watch retains the most recent 32 closed workout identifiers and their saved measurement summaries for delivery retries. The phone retains the most recent 64 command receipts.

## Storage and sharing

GymM8 uses local watch and iPhone storage for this integration. Workout messages travel between your paired devices through Garmin's Connect IQ messaging. The integration has no developer-operated server, advertising or analytics service, and does not send your workout or heart-rate measurements to the developer.

Saved watch activities can sync to your Garmin Connect account through Garmin's normal sync services. Garmin handles that data under its [Garmin Connect privacy policy](https://www.garmin.com/en-US/privacy/connect/policy/). GymM8's full app backups include saved Garmin workout measurements when you choose to export a backup; you control where that file is saved or shared.

## Your choices

Enable or disable workout syncing in GymM8's Garmin settings. Stop and save a recording, or abandon a phone workout to discard its recording. You can delete workout history in GymM8 and saved activities in Garmin Connect separately. Deleting one does not automatically delete the other. Uninstalling the companion removes its app-local data; activities already saved to Garmin Connect remain in your Garmin account.

## Contact

Use the Contact Developer option on the [GymM8 Connect IQ listing](https://apps.garmin.com/apps/cd93a666-cf8e-4082-bced-56e430c06803).

## Apple Health and Apple Watch measurements

Apple Health support in GymM8 is optional. In Settings → Apple Health, choose whether GymM8 may save completed strength workouts and whether it may read workout measurements. Apple's permission sheet lets you choose access to Workouts, Heart Rate and Active Energy Burned. GymM8 does not request clinical records, routes or body-weight data for this integration.

When reading is enabled, GymM8 reads measurements during the workout's start and end times, preferring Apple Watch measurements when available. It displays active calories and average/maximum heart rate with their sources. Imported Health measurements are held in memory; they are not added to GymM8's SwiftData/CloudKit database or exported app backups. They are not sent to the developer, advertisers or an analytics service.

When saving is enabled, GymM8 writes a Traditional Strength Training workout with the real dates, accumulated duration, workout name and a stable identifier to your Apple Health store. It checks for a matching existing workout to avoid duplicate exports. It does not create additional calorie or heart-rate samples from Garmin summary values. Local app storage keeps export identifiers and delivery receipts so retries do not create repeated GymM8 workouts.

Apple Watch recordings and their transfer to Apple Health are handled by Apple's Workout and Health apps. This version does not launch an Apple Watch recording automatically. You can revoke GymM8's permissions in Apple Health and turn the integration off in GymM8. Deleting a GymM8 workout does not automatically delete its Apple Health record; manage those records separately in Health.
